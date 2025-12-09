---
title: "Blog 2"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---


# **Transforming SAP Technical Documentation with GenAI: Accelerating knowledge generation for SAP Notes with Amazon Bedrock**

**This blog was made by Zhang Wenju, Abhi Shivaditya, Beth Sharp, and Zhenyu Yin on 23 SEP 2025**

**This post was jointly authored by AWS and SAP**

### **What are SAP Notes?**

SAP Notes and Knowledge Base Articles (KBA) are fundamental components of SAP’s support ecosystem. These documents provide detailed instructions and solutions for known issues within SAP software products. While SAP Notes primarily focus on coding corrections and technical solutions, KBAs complement them by describing issues in business language, often including screenshots and visual aids. Together, they form a comprehensive knowledge base that helps users and consultants effectively troubleshoot and resolve SAP-related challenges.

---

### **Challenges faced by customers in navigating complex SAP systems and documentation**

As SAP professionals increasingly adopt mobile-first workflows for on-the-go troubleshooting, accessing critical documentation like SAP Notes poses a growing challenge. While users now expect to search and retrieve SAP Notes instantly via smartphones or tablets, the content remains optimized for desktop browsers—forcing mobile viewers to endure excessive zooming, scrolling, and text-heavy navigation. Key implementation steps or urgent configuration fixes are buried in dense technical jargon and multi-page layouts unsuited to compact screens. This disconnect delays time-sensitive resolutions, as support teams waste minutes deciphering desktop-formatted content on mobile devices, increasing the risk of oversight and cognitive fatigue during critical tasks.

---

### **What is the summarization feature that the SAP for Me team introduced?**



---

To address these challenges, the SAP for Me team partnered with AWS. Using Amazon Bedrock, they developed a new version of their mobile app featuring AI-generated summaries of SAP Notes and KBAs. This innovation allows users to quickly navigate and understand technical documentation through concise, automatically generated summaries.

---

### Why is this summarization feature useful for users of the SAP for Me Mobile app?

With the summarization feature, users can quickly assess note relevance for specific business scenarios and access prerequisites and implementation requirements instantly. The feature transforms lengthy technical documentation into mobile-friendly content, highlighting key implementation steps without extensive scrolling thereby significantly reducing time spent during urgent troubleshooting scenarios. End users, for example Basis and functional support teams and consultants, benefit from improved efficiency while on the go, while expert knowledge becomes more accessible in mobile-first contexts, enabling faster decision-making and providing the ability to quickly determine note relevance for investigation.                                |

---

### Laying the foundation: from vision to first deployment

##### Think big and start small

After the Amazon Bedrock integration into SAP’s Generative AI Hub, featuring Claude 3.5 Sonnet and Amazon Titan, was announced at SAP Sapphire in 2024, AWS initiated Generative AI workshops with SAP China Labs. The AWS and SAP China labs fostered a collaborative environment through regular workshops, identifying SAP notes and KBAs, comprising millions of technical documents, as prime candidates for Generative AI enhancement. The teams established weekly meetings and on-demand support to implement SAP Generative AI Hub and invoking Claude models via Amazon Bedrock APIs. Despite initial technical challenges, AWS technical assistance helped SAP meet their pre-Christmas 2024 deployment deadline.

##### What were the initial blockers the team faced?

The team faced time pressure when attempting to summarize 6 million SAP Notes within tight timeframes. Ensuring technical accuracy of AI-generated summaries proved crucial, as did developing efficient systems for managing summarization updates for both new and existing notes.

---

### Architecture Deep Dive: Knowledge bases as a backbone

This project uses retrieval-augmented generation (RAG) to provide customers with precise answers to their queries directly from SAP Notes and KBAs, eliminating the need to manually search through multiple documents. Customers benefit from immediate access to accurate and relevant information, significantly accelerating issue resolution.

The RAG system begins with data ingestion and processing pipeline tailored to SAP Notes and KBAs. In this phase, unstructured and semi-structured documents like SAP notes in html format were systematically collected, cleansed, and transformed into a retrievable format. Key steps include extracting text, metadata (e.g., note numbers, applicability, release versions), and resolving cross-references between documents. Preprocessing techniques, such as semantic chunking and entity recognition, are applied to segment content into contextually meaningful units, while preserving technical nuances. These chunks were then encoded into high-dimensional vector embeddings using Amazon Titan Embedding model. The processed data was indexed in HANA vector database, optimized for fast similarity searches, ensuring the system can efficiently map user queries to the most relevant SAP content during retrieval.

During the query phase, the RAG service combines retrieval and generation to deliver precise answers. When a user submits a query, the system first leverages the HANA vector database to retrieve the top-k SAP Notes or KBA snippets semantically aligned with the query intent. A reranking step prioritizes results based on relevance scores, publication dates, or applicability criteria to ensure up-to-date and actionable insights. The retrieved context is then fed into Bedrock Claude 3.5 Sonnet model via SAP Generative AI Hub into Amazon Bedrock, which synthesizes a concise, natural language response. Crucially, the response is grounded strictly in the retrieved sources, with built-in citations to original notes/KBAs for transparency. This hybrid approach balances speed and accuracy, allowing customers to resolve issues in real time while minimizing hallucinations, thereby reducing reliance on traditional support channels.

---

### Customer value & benefit

SAP’s initiatives to enhance the customer experience through the “Summary for SAP Notes/KBA” and “RAG for SAP Notes/KBA” projects provide significant business value. The two projects streamline access to critical information, enabling customers to efficiently resolve issues and maximize their use of SAP software products. By improving clarity and accessibility, customers can quickly identify relevant solutions, thus reducing downtime and optimizing productivity. This enhanced access to precise information not only improves operational efficiency but also strengthens the overall customer support experience. 

---

### Next step: online recommendations with context

The SAP for Me team is moving from basic summarization to using agentic RAG and knowledge graphs. This will help provide smarter, context-aware technical guidance and make it easier to visualize system dependencies and knowledge map. The team is also working on adding predictive support and personalized recommendations to improve the user experience even more. These steps will build a more powerful and intuitive support system for SAP users.

---

### Conclusion

SAP for Me’s Generative AI journey demonstrates the transformative impact of thoughtfully applying AI to enterprise software challenges. Leveraging the integration of Amazon Bedrock’s Claude 3.5 Sonnet with SAP’s Generative AI Hub, the team tackled the fundamental problem of knowledge accessibility by implementing summarization capabilities for SAP’s vast repository of technical notes. This initial feature addressed the critical need for efficient mobile consumption of complex documentation.

Despite early implementation challenges, including Generative AI upskilling and ensuring technical accuracy, the collaborative effort between SAP and AWS teams successfully delivered the summarization feature before the targeted 2024 year-end holiday deadline. This achievement represents more than just a technical milestone; it marks a fundamental shift in how SAP customers can access and utilize critical technical knowledge on mobile devices.

The roadmap ahead, progressing through agentic RAG, knowledge graph, and proactive recommendations, shows a strategic vision for evolving from static documentation to dynamic, interconnected, and anticipatory knowledge systems. This evolution promises to transform SAP’s customer support model from reactive problem-solving to proactive guidance tailored to each customer’s unique environment.

We encourage you to explore these new capabilities of SAP for Me mobile application and see firsthand how Generative AI can transform your technical support and knowledge management. Reach out to us to learn how you can leverage Amazon Bedrock and unlock greater efficiency and insight for your organization.

**Original blog site**: [Transforming SAP Technical Documentation with GenAI](https://aws.amazon.com/blogs/awsforsap/transforming-sap-technical-documentation-with-genai-accelerating-knowledge-generation-for-sap-notes-with-amazon-bedrock/)
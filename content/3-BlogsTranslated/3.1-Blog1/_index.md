---
title: "Blog 1"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# **IMF chatbot Myelo transforms cancer support with AWS Bedrock and Max.AI**

**by Sapna Kumar and Nickee DeLeon on 23 SEP 2025 in Amazon Bedrock, Artificial Intelligence, Customer Solutions, Generative AI, Healthcare, Nonprofit, Public Sector**

![](media/img1.png)

Founded in 1990, the International Myeloma Foundation (IMF) is the first and largest global foundation focused specifically on multiple myeloma. The IMF’s mission is to improve the quality of life of myeloma patients while working toward prevention and a cure by focusing on four key areas: research, education, support, and advocacy. In September 2024, the IMF launched Myelo—an artificial intelligence-powered virtual assistant built using Amazon Web Services (AWS) and Max.AI, developed by ZS Associates.

This blog post highlights Myelo’s capabilities to provide myeloma patients, caregivers, and healthcare professionals a trustworthy, round-the-clock source of information that is accessible from anywhere in the world, grounded in empathy, and can communicate in multiple languages.

## Generative AI: Closing the gap by disseminating timely information

---
For 35 years, the IMF has been supporting patients’ informational needs through its extensive library of over 100 multilingual publications, a robust website, and a highly trained InfoLine team that answers questions by phone and email.

However, the IMF needed to keep up with the rapid influx of new information (about research, treatments, drug approvals, etc.), manage its ever-growing content, and deliver quick, personalized information to the myeloma community it serves.

The onset of generative AI technology effectively and efficiently filled this need, and Myelo has become the IMF’s dependable AI-powered chatbot—addressing questions and providing information specific to multiple myeloma in a swift, accurate, and empathetic manner.

Myelo uses generative AI to search and synthesize information across the IMF’s deep knowledge base, including web pages, PDFs, videos, and podcasts. It delivers professional, accurate, and compassionate responses—from treatment options and clinical trials to symptom management and diagnosis—within seconds.

Myelo is multilingual and available 24/7, 365 days a year—making it a lifeline for patients and caregivers who need to make complex decisions at any time. As myeloma patient and support group leader Oya Gilbert said: “Having that ability to go onto and talk to Myelo and know that you’re getting a trusted resource, that’s the key—a trusted resource from an organization that is trusted throughout the world, not just in the United States.”

While Myelo can break down complex medical terms into more comprehensible information, it is important to note that it does not offer medical advice or diagnoses. Users are still encouraged to consult healthcare professionals for personalized care.

---

## **AWS Bedrock: The strong foundation that sustains Myelo**


---

Myelo is built on Amazon Bedrock, a service that allows organizations to build and scale generative AI applications using foundational models (FMs)—large language models pre-trained on vast datasets. Bedrock eliminates the need for infrastructure management or model training from scratch, enabling the IMF to move quickly and securely.

At the heart of Myelo’s language processing capabilities is Anthropic’s Claude, a state-of-the-art large language model accessed through AWS Bedrock. Claude’s advanced reasoning abilities and focus on safety make it particularly well-suited for healthcare applications, providing nuanced understanding of medical terminology while maintaining appropriate boundaries around medical advice.

With Bedrock and Claude, the IMF can deploy tools for real-time summarization, question-answering, text classification, and information retrieval—all fine-tuned with the foundation’s own data.

---

## **TMax.AI: Delivering smart, empathetic responses**
---

At the core of Myelo’s intelligence is Max.AI—an enterprise-grade AI platform created by ZS Associates and integrated with AWS services. Max.AI enables Myelo to process and organize large volumes of unstructured content—from transcripts and PDFs to web articles—so users get rich, accurate responses with citations.

The combination of Max.AI’s enterprise capabilities with Claude’s sophisticated language understanding creates a powerful synergy. Max.AI handles the complex data orchestration and content management, while Claude processes natural language queries and generates contextually appropriate responses that maintain the empathetic tone essential for cancer patient support.

Max.AI also allows Myelo to maintain conversation history, delivering contextual, personalized responses over the course of a chat. The platform supports a seamless user experience across all devices, and users can even download their chat transcripts for reference.

Equipped with built-in ethical safeguards and responsible AI protocols, Max.AI ensures that every response Myelo gives is both secure and trustworthy.
---

## Myelo: Breaking barriers and expanding the IMF’s global reach

---

Since its launch, Myelo has become a staple of the IMF’s website, where it appears as a conspicuous pop-up. Users have asked it everything from “What are the infection prevention guidelines for myeloma patients?” to “What does it mean when my FISH chromosome analysis says, ‘Quantity Not Sufficient’?” In 2024 alone, Myelo fielded 16,883 inquiries. In the first half of 2025, it had already responded to more than 55,000.

By addressing many urgent and frequently asked questions, Myelo has enabled the IMF’s InfoLine team to handle more complex, one-on-one needs. Its multilingual capacity has significantly expanded the IMF’s global reach.

One US-based physician praised Myelo after testing it in Spanish: “There was not one question in the session that got an incorrect answer. AMAZING!”

---

## What’s next for Myelo?

---

While Myelo has been successfully delivered, it is merely one milestone on IMF’s digital transformation journey. The chatbot continues to improve based on user feedback, including “thumbs down” ratings that trigger internal review and optimization.

Soon, Myelo will be able to:

Personalize responses based on user profiles and prior chats
Tailor information using geofencing (location-based customization)
Take digital actions on behalf of users via AI agents
Understand and respond to more nuanced or complex medical queries
Offer a voice interface, adding speech recognition and synthesis capabilities
Lay the foundation for the Myeloma Knowledge Platform
Additionally, a version of Myelo to serve solely the healthcare professional community is being developed. Furthermore, Myelo is one part of a larger digital ecosystem the IMF is building: the Myeloma Knowledge Platform (MKP). Built on AWS Data Lake for Nonprofits, the MKP connects Myelo with other tools—such as a clinical trial finder—and unlocks insights by analyzing previously siloed data.

By identifying patterns across these systems, the MKP will offer personalized recommendations to patients, helping them navigate their unique myeloma journeys with greater clarity and confidence.
---

## Front Door Microservice

- Provides an API Gateway for external REST interaction  
- Authentication & authorization based on **OIDC** via **Amazon Cognito**  
- Self-managed *deduplication* mechanism using DynamoDB instead of SNS FIFO because:  
  1. SNS deduplication TTL is only 5 minutes  
  2. SNS FIFO requires SQS FIFO  
  3. Ability to proactively notify the sender that the message is a duplicate  

---

## A more connected, personalized, and patient-centered future

---

As the IMF continues to innovate at the intersection of healthcare and technology, Myelo stands as a compelling example of how generative AI can be used responsibly to empower patients, support caregivers, and ease the burden of a complex disease.

By delivering timely, trusted information with compassion, Myelo is more than just a chatbot: It’s a digital companion helping people make sense of life with myeloma. As part of the broader Myeloma Knowledge Platform, Myelo marks the beginning of a more connected, personalized, and patient-centered future in cancer care.

The IMF believes that by arming patients with knowledge about myeloma, they can make informed decisions about their care, gain access to myeloma specialists in their areas, find the best treatments available to them, and learn practical tools to live well with the disease.

This very much aligns with the IMF’s vision: “A world where every myeloma patient can live life to the fullest, unburdened by the disease.”

---

## About Author

* -Sapna Kumar
  * For six years, Sapna has served as the IMF's manager of marketing and communications. She brings editorial expertise from the publishing industry, from roles at companies including McGraw-Hill, Pearson Education, and Encyclopedia Britannica. In 2021, she served as a digital learning manager with the American Academy of Physical Medicine & Rehabilitation, where she worked with medical professionals to develop continuing medical education courses. She holds a B.A. in writing from Purdue University and certificates in digital marketing, Google Analytics, and web-based communications. In the fall of 2022, she rejoined the IMF team to return to focusing on mission-driven work, always with the patients, caregivers, and the myeloma community at top of mind.

* Nickee DeLeon
  * Nickee is an editorial consultant. She is a versatile creative professional with a proven track record across multiple disciplines in communications and design. With extensive experience spanning publishing, editorial work, writing, graphic design, and art direction, Nickee brings a comprehensive understanding of how visual and written content work together to create compelling narratives.

**Original blog site**: [IMF chatbot Myelo transforms cancer support with AWS Bedrock and Max.AI](https://aws.amazon.com/blogs/publicsector/imf-chatbot-myelo-transforms-cancer-support-with-aws-bedrock-and-max-ai/)
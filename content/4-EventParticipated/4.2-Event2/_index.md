---
title: "Event 2"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# Summary Report: "DevOps on AWS"

### Event Objectives

- Introduce DevOps culture, principles, and key metrics
- Demonstrate AWS DevOps services for CI/CD pipeline automation
- Explore Infrastructure as Code (IaC) with CloudFormation and CDK
- Cover container services and microservices deployment strategies
- Provide monitoring and observability best practices
- Share real-world DevOps case studies and best practices

### Event Details

- **Date**: Monday, November 17, 2025
- **Time**: 8:30 AM – 5:00 PM
- **Location**: Bitexco Financial Tower, 2 Đ. Hải Triều, Bến Nghé, Quận 1, Thành phố Hồ Chí Minh
- **Duration**: Full day (8.5 hours with breaks)

### Agenda

#### Morning Session (8:30 AM – 12:00 PM)

**8:30 – 9:00 AM | Welcome & DevOps Mindset**

- Recap of AI/ML session
- DevOps culture and principles
- Benefits and key metrics (DORA, MTTR, deployment frequency)

**9:00 – 10:30 AM | AWS DevOps Services – CI/CD Pipeline**

- **Source Control**: AWS CodeCommit, Git strategies (GitFlow, Trunk-based)
- **Build & Test**: CodeBuild configuration, testing pipelines
- **Deployment**: CodeDeploy with Blue/Green, Canary, and Rolling updates
- **Orchestration**: CodePipeline automation
- **Demo**: Full CI/CD pipeline walkthrough

**10:30 – 10:45 AM | Break**

**10:45 AM – 12:00 PM | Infrastructure as Code (IaC)**

- **AWS CloudFormation**: Templates, stacks, and drift detection
- **AWS CDK (Cloud Development Kit)**: Constructs, reusable patterns, and language support
- **Demo**: Deploying with CloudFormation and CDK
- **Discussion**: Choosing between IaC tools

#### Lunch Break (12:00 – 1:00 PM)

#### Afternoon Session (1:00 – 5:00 PM)

**1:00 – 2:30 PM | Container Services on AWS**

- **Docker Fundamentals**: Microservices and containerization
- **Amazon ECR**: Image storage, scanning, lifecycle policies
- **Amazon ECS & EKS**: Deployment strategies, scaling, and orchestration
- **AWS App Runner**: Simplified container deployment
- **Demo & Case Study**: Microservices deployment comparison

**2:30 – 2:45 PM | Break**

**2:45 – 4:00 PM | Monitoring & Observability**

- **CloudWatch**: Metrics, logs, alarms, and dashboards
- **AWS X-Ray**: Distributed tracing and performance insights
- **Demo**: Full-stack observability setup
- **Best Practices**: Alerting, dashboards, and on-call processes

**4:00 – 4:45 PM | DevOps Best Practices & Case Studies**

- Deployment strategies: Feature flags, A/B testing
- Automated testing and CI/CD integration
- Incident management and postmortems
- Case Studies: Startups and enterprise DevOps transformations

**4:45 – 5:00 PM | Q&A & Wrap-up**

- DevOps career pathways
- AWS certification roadmap

### Key Highlights

#### DevOps Culture and Principles

- **DevOps Mindset**: Collaboration between development and operations teams
- **Cultural Transformation**: Breaking down silos and fostering shared responsibility
- **Key Metrics (DORA)**: Measuring DevOps performance
  - **Deployment Frequency**: How often deployments occur
  - **Lead Time**: Time from code commit to production
  - **MTTR (Mean Time To Recovery)**: Time to recover from failures
  - **Change Failure Rate**: Percentage of deployments causing failures
- **Benefits**: Faster delivery, improved reliability, better collaboration

#### AWS CI/CD Pipeline Services

**AWS CodeCommit:**

- Fully managed source control service
- Git-based version control
- Integration with other AWS services
- Git strategies: GitFlow, Trunk-based development, feature branches

**AWS CodeBuild:**

- Fully managed build service
- Scalable build environments
- Supports multiple programming languages and build tools
- Build artifacts and test reports
- Integration with testing frameworks

**AWS CodeDeploy:**

- Automated deployment service
- Deployment strategies:
  - **Blue/Green**: Zero-downtime deployments with instant rollback
  - **Canary**: Gradual rollout with automatic rollback on errors
  - **Rolling**: Rolling updates with configurable batch sizes
- Application deployment across EC2, Lambda, and on-premises

**AWS CodePipeline:**

- Fully managed continuous delivery service
- Visual workflow builder
- Integration with third-party tools
- Automated pipeline orchestration
- Approval gates and manual intervention points

#### Infrastructure as Code (IaC)

**AWS CloudFormation:**

- Declarative IaC service
- JSON/YAML template syntax
- Stack management and resource provisioning
- Drift detection and stack updates
- Change sets for previewing changes
- Nested stacks for modular infrastructure

**AWS CDK (Cloud Development Kit):**

- Programmatic IaC using familiar programming languages
- TypeScript, Python, Java, C#, and Go support
- Constructs for reusable infrastructure patterns
- Higher-level abstractions and best practices
- Integration with CloudFormation
- CLI tools for deployment and management

**Choosing Between IaC Tools:**

- CloudFormation: Declarative, template-based, AWS-native
- CDK: Programmatic, type-safe, developer-friendly
- Use cases and when to choose each approach

#### Container Services on AWS

**Docker Fundamentals:**

- Containerization benefits and use cases
- Microservices architecture with containers
- Docker image creation and optimization
- Multi-stage builds and best practices

**Amazon ECR (Elastic Container Registry):**

- Fully managed Docker container registry
- Image storage and versioning
- Image scanning for vulnerabilities
- Lifecycle policies for automated cleanup
- Integration with ECS and EKS

**Amazon ECS (Elastic Container Service):**

- Fully managed container orchestration
- Fargate (serverless) and EC2 launch types
- Task definitions and service configurations
- Auto-scaling and load balancing
- Service discovery and networking

**Amazon EKS (Elastic Kubernetes Service):**

- Managed Kubernetes service
- Kubernetes-native orchestration
- Worker nodes management
- Add-ons and ecosystem integration
- Multi-tenant and namespace isolation

**AWS App Runner:**

- Simplified container deployment
- Automatic scaling and load balancing
- Source code or container image deployment
- Built-in CI/CD integration
- Pay-per-use pricing model

#### Monitoring & Observability

**Amazon CloudWatch:**

- **Metrics**: Application and infrastructure metrics
- **Logs**: Centralized log management and analysis
- **Alarms**: Automated alerting and notifications
- **Dashboards**: Custom visualization of metrics and logs
- **Insights**: Automated anomaly detection
- **Composite Alarms**: Complex alerting logic

**AWS X-Ray:**

- Distributed tracing for microservices
- Request flow visualization
- Performance bottleneck identification
- Service map generation
- Integration with Lambda, ECS, and API Gateway
- Trace analysis and filtering

**Best Practices:**

- Setting up effective alerting strategies
- Creating meaningful dashboards
- On-call processes and incident response
- Log aggregation and analysis
- Metric collection and retention policies

#### DevOps Best Practices

**Deployment Strategies:**

- **Feature Flags**: Gradual feature rollouts
- **A/B Testing**: Comparing different versions
- **Canary Deployments**: Risk mitigation through gradual rollout
- **Blue/Green Deployments**: Zero-downtime updates

**Automated Testing:**

- Unit, integration, and end-to-end testing
- Test automation in CI/CD pipelines
- Quality gates and test coverage
- Performance and load testing

**Incident Management:**

- Runbook creation and maintenance
- Incident response procedures
- Postmortem analysis and learning
- Continuous improvement processes

### Key Takeaways

#### DevOps Culture Transformation

- **Cultural Change is Fundamental**: Tools alone don't make DevOps—culture and collaboration are key
- **Measure What Matters**: Use DORA metrics to track DevOps maturity
- **Continuous Improvement**: DevOps is a journey, not a destination
- **Automation First**: Automate repetitive tasks to focus on high-value work

#### CI/CD Best Practices

- **Start Simple, Scale Gradually**: Begin with basic pipelines and add complexity over time
- **Git Strategy Matters**: Choose GitFlow or Trunk-based based on team size and release cadence
- **Testing is Critical**: Integrate automated testing at every stage
- **Deployment Strategies**: Use appropriate deployment strategy based on risk tolerance
- **Infrastructure as Code**: Always use IaC for reproducible and version-controlled infrastructure

#### Container Orchestration

- **Choose Wisely**: ECS for simplicity, EKS for Kubernetes ecosystem
- **Start with Serverless**: Fargate eliminates node management overhead
- **Optimize Images**: Smaller images mean faster deployments and lower costs
- **Security First**: Scan images and use least-privilege IAM policies

#### Observability Strategy

- **Implement Full-Stack Observability**: Metrics, logs, and traces together
- **Proactive Monitoring**: Set up alarms before incidents occur
- **Meaningful Dashboards**: Create dashboards that provide actionable insights
- **Distributed Tracing**: Essential for debugging microservices architectures

### Applying to Work

- **Implement CI/CD Pipelines**: Set up CodePipeline for automated deployments
- **Adopt Infrastructure as Code**: Use CloudFormation or CDK for all infrastructure
- **Containerize Applications**: Start containerizing applications for better portability
- **Set Up Monitoring**: Implement CloudWatch and X-Ray for observability
- **Establish DevOps Practices**: Create runbooks, incident response procedures, and postmortem templates
- **Measure DevOps Metrics**: Track DORA metrics to measure improvement

### Event Experience

Attending the **"DevOps on AWS"** full-day workshop was an intensive and comprehensive learning experience that covered the entire DevOps spectrum from culture to implementation. The event provided both theoretical knowledge and practical demonstrations, giving me a complete understanding of implementing DevOps practices on AWS.

#### Learning DevOps fundamentals

- The session started with **DevOps mindset and culture**, emphasizing that DevOps is more than just tools—it's about collaboration and shared responsibility.
- I learned about **DORA metrics** (Deployment Frequency, Lead Time, MTTR, Change Failure Rate) and how to measure DevOps maturity.
- Understanding the **benefits of DevOps** helped me see the bigger picture beyond technical implementation.

#### AWS CI/CD pipeline deep dive

- The **CodeCommit, CodeBuild, CodeDeploy, and CodePipeline** walkthrough showed me how to build a complete CI/CD pipeline.
- Learning about different **Git strategies** (GitFlow vs Trunk-based) helped me understand when to use each approach.
- The **deployment strategies** (Blue/Green, Canary, Rolling) demo was eye-opening, showing how to minimize risk and downtime.
- The live **CI/CD pipeline demo** demonstrated the entire workflow from code commit to production deployment.

#### Infrastructure as Code mastery

- **CloudFormation** demonstrated how to manage infrastructure declaratively with templates.
- **AWS CDK** showed me how to write infrastructure code in familiar programming languages, making it more maintainable.
- The comparison between CloudFormation and CDK helped me understand when to use each tool.
- Learning about **drift detection** and **change sets** gave me confidence in managing infrastructure safely.

#### Container services exploration

- **Docker fundamentals** refreshed my understanding of containerization and its benefits.
- **Amazon ECR** showed how to manage container images securely with scanning and lifecycle policies.
- Comparing **ECS and EKS** helped me understand the trade-offs between managed services and Kubernetes flexibility.
- **AWS App Runner** introduced a simpler way to deploy containers without managing infrastructure.
- The **microservices deployment case study** provided real-world insights into choosing the right container service.

#### Monitoring and observability setup

- **CloudWatch** comprehensive coverage showed me how to collect metrics, logs, and set up alarms.
- **AWS X-Ray** distributed tracing demonstrated how to debug complex microservices architectures.
- The **full-stack observability demo** showed how to connect all monitoring pieces together.
- Learning about **alerting best practices** and **on-call processes** provided practical operational knowledge.

#### Best practices and case studies

- **Deployment strategies** like feature flags and A/B testing showed advanced techniques for safe deployments.
- **Automated testing integration** demonstrated how to build quality gates into CI/CD pipelines.
- **Incident management** practices and postmortem templates provided structure for handling production issues.
- **Case studies** from startups and enterprises showed real-world DevOps transformations and lessons learned.

#### Career and certification guidance

- The **DevOps career pathways** discussion helped me understand different roles and skill requirements.
- The **AWS certification roadmap** provided clear guidance on certifications relevant to DevOps.
- Understanding the career progression gave me a roadmap for professional development.

#### Practical demonstrations

- Every session included **live demos** that showed real implementations, not just slides.
- The **full CI/CD pipeline walkthrough** demonstrated end-to-end automation.
- **CloudFormation and CDK demos** showed both approaches to infrastructure management.
- **Container deployment comparison** helped me visualize different approaches side by side.

#### Networking and discussions

- The full-day format allowed for **extended networking** with other DevOps practitioners.
- **Q&A sessions** provided opportunities to get answers to specific questions.
- Discussing **real-world challenges** with peers helped me understand common pitfalls and solutions.

#### Lessons learned

- **DevOps is a cultural transformation** that requires buy-in from both development and operations teams.
- **Automation is essential** but must be implemented thoughtfully to avoid creating technical debt.
- **Infrastructure as Code** is non-negotiable for modern DevOps practices.
- **Monitoring and observability** are crucial for maintaining production systems.
- **Start simple and iterate** rather than trying to implement everything at once.
- **Measure everything** using DORA metrics to track improvement over time.

  #### Some event photos
  
![Event Photo 1](image/z7256923076166_a5096f1705aa25115465f612c36c5b25.jpg)

![Event Photo 2](image/z7256923087749_1dc51ba7fd23c4977ea952e46c0e0826.jpg)

![Event Photo 3](image/z7256923095334_4155afecb768541621090af29d7aaeff.jpg)
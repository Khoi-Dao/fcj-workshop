---
title: "Week 8 Worklog"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---



### Week 8 Objectives:

* Complete the Edge Layer and Frontend Storage: Route 53, S3, CloudFront, AWS WAF, and ACM Certificate.
* Set up DNS management with Route 53 hosted zone and domain configuration.
* Configure S3 bucket for static frontend hosting with proper access policies.
* Deploy CloudFront distribution for global content delivery with Origin Access Control.
* Implement AWS WAF protection with security rules (SQL injection, XSS, bot control).
* Set up ACM Certificate and enable HTTPS for secure content delivery.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - System Requirements Analysis & Architecture Design: <br>&emsp; + Analyze system requirements and review the complete architecture diagram. <br>&emsp; + Identify all components: Route 53, S3, CloudFront, WAF, ACM, VPC, EC2, RDS, API Gateway. <br>&emsp; + Create High-Level Design (HLD) document with architecture overview. <br>&emsp; + Document data flow: Users → Route 53 → CloudFront → WAF → S3 (Frontend). <br>&emsp; +  Plan IP addressing scheme and resource naming conventions.                                                                                                  | 10/26/2025 | 10/26/2025      | Architecture diagram |
| 3   | - Route 53 Setup: <br>&emsp; + Create Route 53 hosted zone for domain management. <br>&emsp; + Create A record pointing to CloudFront distribution  <br>&emsp; +  Create CNAME records for subdomains if needed. <br>&emsp; + Configure DNS settings and verify domain ownership. <br>&emsp; + Document DNS configuration and record types. <br> - S3 Frontend Bucket Configuration: <br>&emsp; + Create S3 bucket for frontend static assets (FE Bucket) with appropriate naming. <br>&emsp; + Enable static website hosting on S3 bucket. <br>&emsp; + Configure public access policy for CloudFront access (block public access, allow CloudFront via OAC). <br>&emsp; + Upload test frontend files (HTML, CSS, JS, images) to S3 bucket. <br>&emsp; + Test static website hosting endpoint and verify file accessibility.                                             | 10/27/2025 | 10/27/2025      | Route 53 documentation <br> S3 documentation |
| 4   | - CloudFront Distribution Setup: <br>&emsp; + Create CloudFront distribution with S3 bucket as origin. <br>&emsp; + Configure Origin Access Control (OAC) for secure S3 access (replacing OAI). <br>&emsp; + Set up cache policies (CachingOptimized, CachingDisabled, etc.). <br>&emsp; + Configure default root object (index.html). <br>&emsp; + Map Route 53 domain to CloudFront distribution . <br>&emsp; + Test CloudFront distribution and verify content delivery. | 10/28/2025 | 10/28/2025      | CloudFront documentation |
| 5   | - AWS WAF Integration: <br>&emsp; + Create AWS WAF WebACL for CloudFront protection. <br>&emsp; + Add managed rules: AWS Managed Rules for SQL injection protection. <br>&emsp; + Add managed rules: AWS Managed Rules for XSS (Cross-Site Scripting) protection. <br>&emsp; + Configure bot control rules to block common bots and scrapers. <br>&emsp; + Associate WAF WebACL with CloudFront distribution. <br>&emsp; +  Test WAF rules by attempting common attack patterns and verify blocking.                           | 10/29/2025 | 10/29/2025      | AWS WAF documentation |
| 6   | - AWS WAF Integration: <br>&emsp; +  Request ACM Certificate in us-east-1 region (required for CloudFront). <br>&emsp; + Validate certificate using DNS validation method (add CNAME records to Route 53). <br>&emsp; + Wait for certificate validation and issuance. <br>&emsp; + Bind ACM certificate to CloudFront distribution. <br>&emsp; +  Configure CloudFront to use HTTPS only (redirect HTTP to HTTPS). <br>&emsp; +  Test HTTPS connection and verify SSL/TLS certificate is working correctly.                                                                                   | 10/30/2025 | 10/30/2025      | ACM documentation |


### Week 8 Achievements:

* Successfully completed system analysis and architecture design:

  * Analyzed system requirements and reviewed complete architecture diagram.
  * Created High-Level Design (HLD) document with architecture overview and component relationships.
  * Documented data flow from users through edge services to frontend storage.
  * Established resource naming conventions and planning documentation.
* Set up Route 53 DNS management:

  * Created Route 53 hosted zone for domain management.
  * Configured A and CNAME records for domain routing.
  * Established DNS foundation for connecting domain to CloudFront distribution.
* Configured S3 for static frontend hosting:

  * Created S3 bucket for frontend static assets with proper naming conventions.
  * Enabled static website hosting on S3 bucket.
  * Configured public access policies: blocked public access, allowed CloudFront access via Origin Access Control.
  * Uploaded test frontend files and verified static website hosting functionality.
* Deployed CloudFront distribution:

  * Created CloudFront distribution with S3 bucket as origin.
  * Configured Origin Access Control (OAC) for secure S3 access (modern replacement for OAI).
  * Set up cache policies for optimized content delivery.
  * Mapped Route 53 domain to CloudFront distribution.
  * Verified content delivery through CloudFront CDN globally.
* Implemented AWS WAF protection:

  * Created AWS WAF WebACL with comprehensive security rules.
  * Added AWS Managed Rules for SQL injection protection.
  * Added AWS Managed Rules for XSS (Cross-Site Scripting) protection.
  * Configured bot control rules to block malicious bots and scrapers.
  * Associated WAF WebACL with CloudFront distribution.
  * Tested WAF rules and verified protection against common attack patterns.
* Enabled HTTPS with ACM Certificate:

  * Requested and validated ACM Certificate in us-east-1 region (required for CloudFront).
  * Used DNS validation method with CNAME records in Route 53.
  * Bound ACM certificate to CloudFront distribution.
  * Configured CloudFront to enforce HTTPS (redirect HTTP to HTTPS).
  * Verified SSL/TLS certificate is working correctly and secure connections are established.

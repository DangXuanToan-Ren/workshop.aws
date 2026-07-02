---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# SUMMARY REPORT: AWS & GENERATIVE AI (EVENT 2)


## I. Event Overview

The event focused on the practical application of AWS services and Generative AI (GenAI) to specialized technical problems. The content spanned from AI optimization techniques (Context Engineering, handling LLM non-determinism), system architecture (CloudFront, Multi-Agent), to real-world product building experiences from Hackathons.


## II. List of Speakers & Topics

- Brother Thịnh: "Context Is Everything - Build Second Brain".
- Brother Hải Anh: "Friendly AI Assistant w/ Amazon Quick".
- Team VIB: "36 hrs with LotusHacks - Building UTMorpho".
- Brother Thịnh: "From Edge To Origin: CloudFront as Your Foundation".
- Brother Đức Đào: "Non-Determinism of Deterministic LLM Settings".
- Sister Vy Lam: "Enterprise-Grade Multi-Agent System".


## III. Key Highlights

### 1. Brother Thịnh — Context Is Everything (Optimizing AI Context)
- Many disappointing AI results stem from poor context provision, not from bad AI models.
- A good context needs to clearly define 4 factors: Goal, Situation, Constraints, and Relevant Evidence/Data.
- Common mistakes to avoid: Don't stuff all messy online data into the prompt ("Internet Puller"), don't ask AI to do obvious things, and don't make vague requests without constraints.
- The future of AI usage is shifting from just writing simple prompts to building "Context Systems" (Prompt → Context → Memory) also known as "Second Brain".


### 2. Brother Hải Anh — Friendly AI Assistant (AI Assistant with Amazon Q)
- Agentic AI models are built based on integrating company data and a safe knowledge space.
- Using an AI assistant helps simplify and accelerate the transition from analyzing information (insight) to taking real action (action).
- The AI assistant can be used as a "PM Assistant" to automate repetitive tasks like: automatically creating meeting minutes (MoM), sending emails to relevant parties and scheduling meetings.


### 3. Team VIB — Building UTMorpho in 36 hours
- Building a product under high pressure requires the team to go through phases: Setup, building the core, facing mid-stage difficulties, and polishing before presentation.
- Real hackathon challenges include: AI generating too much redundant data (Overgeneration), fatigue/exhaustion close to presentation time, and token limits (Token Limits).
- Key lessons learned: Frustration with current solutions is exactly the source of real ideas, and in high-intensity environments, team synchronization (Team Sync) is the most important factor.


### 4. Brother Thịnh — Optimizing Infrastructure with Amazon CloudFront
- Customers often face risks from traffic spikes or cyberattacks, leading to unexpected CDN costs.
- CloudFront provides a security solution with fixed pricing, combined with WAF, DDoS protection, and traffic throttling to eliminate financial risk.
- On the performance side, CloudFront helps reduce origin server load time by supporting multi-stream downloads (HTTP/3 multiplexing) and HTTP data compression, helping reduce up to 81% response time and 82% bandwidth.
- Using CloudFront with Origin Access Control (OAC) or Custom Headers helps hide the origin server (Origin cloaking), increasing system security.


### 5. Brother Đức Đào — Non-Determinism of LLMs
- Even with temperature set to 0 (Temperature = 0) which in theory should produce consistent outputs, real-world LLM models still have variance.
- The deep technical reason comes from hardware architecture (floating-point math on GPUs) and inference batching from API providers to optimize costs.
- Mitigation techniques include: Running the prompt multiple times and taking the most common result (Majority voting), forcing the model to return structured data (JSON mode, Regex), or self-hosting the model.


### 6. Sister Vy Lam — Enterprise-Grade Multi-Agent System
- Traditional simple models often fail when applied to Startups due to slow response times, distributed data and not adapting quickly.
- The Multi-Agent architecture solves this by establishing a "Virtual Council of Trust", where specialized AIs (Financial Analysis, Market Analysis, Risk Assessment...) work in parallel and cross-check each other.
- Enterprise-grade systems require strict security standards (VPC network, IAM management, data encryption) and guardrail control mechanisms at inputs, processing and outputs.
- Applying this architecture delivers impressive ROI: 95% reduction in processing time, 95% cost savings for decisions and increased approval rates.


## IV. Key Values Gained

- About System Optimization: Understood the importance of Origin cloaking and using Edge computing to both reduce resource costs and defend against DDoS attacks.
- About AI & Prompt Engineering: Clearly recognized that nothing is 100% certain in AI (even with Temperature = 0). Providing clean, concise, structured Context is more important than stuffing data into prompts.
- About Development Mindset: In the future, career differences won't be "Humans vs AI", but "People who know how to use AI" vs "People who don't". Building enterprise AI isn't just about making it work—it must be secure, reliable, and scalable.


## V. Plan to Apply in Practice

- Change how we work with LLMs: Apply variance-aware system design by standardizing output formats (like JSON) instead of relying entirely on the model's free text.
- Apply "Guardrails" and least privilege principle when deploying Backend/Cloud projects to ensure security from the architecture design phase.
- Optimize internship and AWS lab projects: Set up CloudFront as a mandatory buffer layer in front of EC2 or S3 servers, configure automatic compression to reduce bandwidth and improve frontend response times.
- Build a personal "Second Brain" system to store, retrieve technical documents, source code and AWS knowledge systematically.


## VI. Personal Reflections

The second event was technically specialized and expanded architectural perspective for those differences. I was particularly impressed with the "Non-Determinism" topic because it clearly explained why there are those undefined errors I encountered when testing LLM APIs. The Multi-Agent and CloudFront presentations also provided very valuable practical best-practices, helping me shape a clearer picture of how large enterprises operate secure infrastructure and integrate AI safely and cost-effectively for software projects.


## VII. Some Event Photos

<img src="/images/Event2/z7969075645797_c6232463de54c809944d4c1fc251693b.jpg" alt="AWS & Generative AI Event Photo 1" class="blog-image" />
<img src="/images/Event2/z7969075646427_3bd1c651ae7b793d115fa3c37c78272f.jpg" alt="AWS & Generative AI Event Photo 2" class="blog-image" />

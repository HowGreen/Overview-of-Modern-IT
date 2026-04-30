\# Overview of Modern IT: An AWS Solutions Architect Study Textbook



A self-directed textbook project for the \*\*AWS Certified Solutions Architect – Associate (SAA-C03)\*\* exam, built over eight months using AI-assisted content generation, original SVG illustrations, and Markdown/Pandoc tooling.



\## About This Project



I came to AWS with a background in on-premises IT (CompTIA A+, Network+, and Security+) but no experience with cloud services or modern IT practrices — databases, containers, web applications, data processing, machine learning workflows, and more were all new territory. Rather than memorize AWS services in isolation, I wanted to understand them as \*\*solutions to real business needs across realistic IT environments\*\*.



I used Claude and Gemini as collaborative writing tools to produce a full-length textbook structured around this idea. The process involved:



\- \*\*Developing a detailed outline\*\* that mapped AWS services and architectural patterns to 9 common IT environments (public-facing apps, data processing, internal systems, dev/test, media production, regulated systems, disaster recovery, AI/ML, and migration/hybrid cloud)

\- \*\*Writing complex prompts\*\* to guide AI models through each section iteratively — proposing structure, reviewing output, requesting revisions, and stitching together approved sections in VSCode

\- \*\*Creating original SVG diagrams\*\* in Inkscape to illustrate architectural concepts

\- \*\*Compiling the final ePub\*\* using Pandoc for reading on a tablet



The textbook uses a narrative voice — an experienced Solutions Architect reflecting on the industry's shift from on-premises to cloud — and frames every AWS service in the context of the Well-Architected Framework pillars: availability, performance, scalability, security, cost optimization, and operational management.



\## Repository Contents



```

├── source/

│   ├── Sections\_1\_and\_2.md       # IT evolution, environments overview, foundational concepts

│   ├── Section3.md               # Deep dives: 9 environments × 6 NFR categories

│   └── images/                   # SVG illustrations (93 diagrams)

├── outline/

│   └── Overview\_of\_Modern\_IT.txt # The master outline that drove the entire project

├── process/

│   └── Project Description3.txt        # Representative version of the prompt used to generate each section

├── output/                       # Compiled ePub (built with Pandoc)

└── README.md

```



\## Textbook Structure



\*\*Section 1 — The Evolution of Modern IT\*\*

Traces the shift from infrastructure-centric to service-centric thinking, surveys 9 IT environment types, and defines foundational concepts (workloads, architecture, non-functional requirements).



\*\*Section 2 — Core Technology Concepts\*\*

Covers compute, networking, storage, databases, the AWS service taxonomy, and decoupling/asynchronous processing patterns.



\*\*Section 3 — Environment Deep Dives\*\* \*(~22,000 lines)\*

Each environment is examined through all six Well-Architected pillars:



| Environment | Section |

|---|---|

| Public-Facing Applications | 3.1 |

| Data Processing \& Analytics | 3.2 |

| Internal Business Systems | 3.3 |

| Development \& Test Environments | 3.4 |

| Media \& Content Production | 3.5 |

| Regulated/Compliance-Driven Systems | 3.6 |

| Disaster Recovery \& Business Continuity | 3.7 |

| AI/ML Development \& Inference | 3.8 |

| Migration \& Hybrid Cloud | 3.9 |



\## Sample Illustrations



The textbook includes 93 original SVG diagrams covering topics like:



\- The 7 R's migration strategy spectrum

\- API Gateway VPC Link architecture

\- API composition patterns

\- Analytics CI/CD pipelines

\- Three-tier architecture patterns

\- Service-centric vs. infrastructure-centric metrics



\## How It Was Built



\### Tools

\- \*\*Claude and Gemini\*\* — AI-assisted content generation through iterative prompting

\- \*\*VSCode\*\* — Primary workspace for writing, editing, and assembling Markdown

\- \*\*Inkscape\*\* — SVG diagram creation and editing

\- \*\*Pandoc\*\* — ePub compilation from Markdown source



\### Build Command

```bash

cd project-directory

pandoc source/Section3.md -o output/Section3.epub \\

&nbsp; --resource-path=.:images/ \\

&nbsp; --css custom-styles.css

```



\### Workflow



1\. \*\*Outline development\*\* — Researched SAA-C03 exam objectives; identified 9 IT environments as the organizing framework; developed detailed Key Discussion Points (KDPs) for each environment/NFR combination through conversations with Claude and Gemini

2\. \*\*Iterative prompting\*\* — For each section, I provided the AI with the relevant KDPs and a structured prompt template. The AI proposed subsection structure; I reviewed and adjusted; it generated text incrementally for my review

3\. \*\*Assembly and editing\*\* — Approved sections were stitched together in VSCode. New AI sessions received context from prior sections to maintain continuity and avoid redundancy

4\. \*\*Illustration\*\* — Created SVG diagrams to accompany the text, learning SVG syntax and Inkscape in the process

5\. \*\*Compilation\*\* — Built the ePub with Pandoc for tablet reading



The project ran from approximately mid-2025 through early 2026.



\## What This Project Demonstrates



\- \*\*Self-directed learning\*\* — Designed and executed a structured study plan for a complex certification

\- \*\*Prompt engineering\*\* — Developed and refined complex prompts to produce consistent, high-quality technical content across many sessions

\- \*\*Project management\*\* — Managed an eight-month project with evolving requirements, iterative review cycles, and a clear deliverable

\- \*\*Technical writing and editing\*\* — Reviewed, revised, and assembled AI-generated content into a coherent 25,000+ line textbook

\- \*\*Technical tooling\*\* — Learned and applied Markdown, Pandoc, SVG/Inkscape, and VSCode for document production



\## Outcome



I passed the AWS Certified Solutions Architect – Associate exam in February 2026.



\## License



This textbook was created for personal study. The content was generated with AI assistance (Claude by Anthropic, Gemini by Google) and edited/assembled by me. It is shared here as a portfolio piece demonstrating the project and process.


# Baha Kırbaşoğlu

AI Engineer at [PEAKUP](https://peakup.org), Türkiye's first and only Microsoft Frontier Partner, and MSc candidate in Computer Engineering at Istanbul Technical University.

I build LLM-agent and document-intelligence systems for enterprise clients in banking, energy, logistics and manufacturing, and take them from scoping to production and handover. Alongside delivery I teach: university AI courses as an adjunct instructor, and corporate AI training in Turkish and English.

## Client work

Client code lives in private repositories. These are the engagements I can describe.

**Nexent Bank (banking).** Three systems for a Swiss bank.

- *KYC onboarding agent* on Copilot Studio and Azure AI Foundry. It researches internal policy and completes the eligibility workbook from the documents a client uploads, answer by answer with its source, replacing a process that took 2 to 3 weeks per client. It is now the relationship managers' standard onboarding workflow.
- *Credit risk platform.* Analysts import a borrower's evidence and run versioned teams of agents over it under supervision; the output is a credit memo and workbook that passes a four-eyes review. Built on FastAPI and React, with LangGraph and a Postgres checkpointer, Azure Service Bus and Container Apps.
- *News-watch agent*, live since August 2026. Every hour it scans the press for the companies on the bank's watch-list and sends one deduplicated digest, or nothing when there is nothing new. In its measured period it did not miss a scheduled hour, filtered out 92% of 4,373 candidate articles before they reached anyone, and scanned 100 clients in 80 seconds. The same engine is exposed to Copilot Studio as an MCP server.

**Enerjisa (energy).** Document-processing pipeline that reads 26 document types, including invoices, notarial deeds and insurance policies, and posts the extracted data to SAP through a custom MCP server. The accounting team now reviews output instead of keying in data.

**CEVA Logistics (logistics).** Two systems, both now standard in the logistics operations unit. An e-mail-to-order agent reads free-form shipment requests, extracts order fields against Pydantic schemas, matches the customer, follows up on missing details and returns the quote; it does the work of one full-time coordinator, about 8 hours a day. A generative-AI OCR pipeline processes about 120,000 trip documents a month across 19 customer-specific templates, on Azure AI Document Intelligence and Azure OpenAI, deployed as serverless Azure Functions.

**SASA Polyester (manufacturing).** WhatsApp agent that answers business questions in natural language by querying Power BI directly, so users get reporting figures without opening a dashboard.

**Flormar (cosmetics).** Corporate knowledge assistant on Copilot Studio over 12 SharePoint sources and about 136 documents, mostly HR. It routes each question to the right source, applies date rules to answer from the current version of a document, and hands sensitive topics to HR.

**A hospital group (healthcare).** Proof of concept for a permission-aware RAG assistant embedded in the intranet. It answers only from the documents the signed-in user is allowed to see and cites its sources. FastAPI, a React widget, Azure AI Search with hybrid retrieval and Azure AI Foundry.

**Kansai Altan (paints).** Azure migration of three internal business applications to App Service for Containers with GitHub Actions, and the engineering standards they now share: naming, CI/CD and branching.

**PEAKUP (internal).** A sector-neutral case-agent platform that generalises the credit risk work: versioned agents and workflows, MCP connections, golden-case evaluations and sector packs for banking, logistics and pharma, installed in each customer's own tenant.

**ZF Friedrichshafen (automotive).** Anomaly detection models for manufacturing quality processes, with SHAP and LIME layers that show engineers why a part was flagged. They held 98 to 99% accuracy on live production data through continuous retraining. Delivered while at NTT DATA Business Solutions.

## Teaching and training

**Corporate AI training.** More than 100 days of training for over 1,000 participants at Eczacıbaşı, TAV, MetLife, Nexent Bank, CEVA Logistics, Hedef Filo, KPMG, Centurion, Petroyağ and Brisa. Sessions run in Turkish or English, in person or online, and are adapted to the audience's sector and departments.

| Programme | Audience | Content |
| --- | --- | --- |
| AI 101 | All employees, half or full day | The history of AI up to transformer architectures, how generative AI works and where it fails, prompt engineering, responsible use, department scenarios |
| Microsoft 365 Copilot | Business departments | Copilot in daily work by department: finance, HR, sales, operations, legal, IT |
| Copilot Studio | Power users and IT | Designing, grounding and publishing agents; hands-on labs with test questions and a prompt-injection demo |
| Azure AI Foundry | Developers and data teams | Building and deploying models and agents on Azure AI Foundry |
| GitHub Copilot and vibe coding | Developers | AI-assisted development with GitHub Copilot, from prompt to working application |

**University teaching.** Adjunct instructor in PEAKUP's Sektör Kampüste programme since 2025, now in its third semester. I teach AI courses at Süleyman Demirel University, Okan University, Kocaeli Health and Technology University and Atatürk University: syllabus and exam design, lectures, student projects and grading.

## Research

MSc thesis at Istanbul Technical University: uncertainty-aware, explainable whole-body PET/CT lesion segmentation with a dual-channel nnU-Net.

**Publication.** "Small-Lesion Detection in Whole-Body FDG PET/CT: A Lesion-Level Audit of Training and Post-Processing Trade-offs", first author, accepted at ISMSIT 2026.

## Repositories

| Project | What it is |
| --- | --- |
| [document-extraction-pipeline](https://github.com/Bahakirbasogluu/document-extraction-pipeline) | Schema-driven document extraction: split, classify, extract into Pydantic schemas, validate against business rules and map to a downstream record. Runs offline on synthetic documents, with an Azure OpenAI backend. |
| [erp-mcp-server](https://github.com/Bahakirbasogluu/erp-mcp-server) | MCP server that gives agents guarded access to an ERP REST API: typed tools, two-step confirmed writes, idempotent posting and errors that say what to do next. Includes a mock ERP. |
| [email-to-order-agent](https://github.com/Bahakirbasogluu/email-to-order-agent) | Agent workflow for an order mailbox: reads free-form shipment requests, asks for missing details, prices from a rate card and hands over to a person when it should not decide. |
| [lesion-level-eval](https://github.com/Bahakirbasogluu/lesion-level-eval) | Lesion-level evaluation of 3D segmentation masks: detection by lesion size, false positives per study and patient-cluster bootstrap intervals. The evaluation method behind my thesis, on synthetic data. |
| [Fraud-Detection](https://github.com/Bahakirbasogluu/Fraud-Detection) | One-class anomaly detectors (OCSVM, GMM, Isolation Forest, LOF) and score ensembles (voting, stacking) for fraud detection on credit card and Medicare data. |
| [Fraud-Detection-GT](https://github.com/Bahakirbasogluu/Fraud-Detection-GT) | The graph-based companion study on the same datasets: centrality and community analysis, spectral methods, and GNNs (GCN, GraphSAGE, GAT, DOMINANT). |
| [IMPBA](https://github.com/Bahakirbasogluu/IMPBA) | Image inpainting for object removal with two U-Net variants, comparing MSE and VGG19 perceptual loss; evaluated with PSNR, SSIM and LPIPS. |
| [docgen_data](https://github.com/Bahakirbasogluu/docgen_data) | Turkish and English technical-support dialogue dataset (341 samples) for issue classification, title generation, sentiment analysis and summarization. |
| [smart-fridge](https://github.com/canatess/smart-fridge) | Undergraduate graduation project: estimating the freshness of produce from visible spoilage. Team project. |

The older repositories on this profile are coursework from my undergraduate years at Hacettepe University.

## Toolbox

**LLM and agents:** Azure OpenAI, Copilot Studio, Azure AI Foundry, LangChain and LangGraph, custom MCP servers, RAG, multi-agent orchestration.

**ML and cloud:** PyTorch, scikit-learn, Hugging Face, nnU-Net, Azure AI Document Intelligence, SHAP and LIME, Azure Functions, Azure Machine Learning, Azure DevOps, Docker, FastAPI.

## Background

- MSc Computer Engineering, Istanbul Technical University (2025 to January 2027, expected)
- BSc Artificial Intelligence Engineering, Hacettepe University (2019 to 2024)
- Microsoft Certified: Azure AI Engineer Associate
- Before PEAKUP: AI Engineer at ONO Teknoloji, building LLM-based chatbots and the software around them
- Data Scientist at NTT DATA Business Solutions: anomaly detection at ZF, and LLM chatbot and agentic proofs of concept for BMW and Nobel

## Writing and speaking

- Articles on applied AI and agentic systems on [Medium](https://medium.com/@bahakirbashov)
- Guest on the PEAKUP Teknoloji Konuşmaları podcast, on multi-agent systems in enterprise workflows

## Contact

[LinkedIn](https://www.linkedin.com/in/bahakirbasoglu) · [Medium](https://medium.com/@bahakirbashov) · [Kaggle](https://www.kaggle.com/bahakirbasoglu)

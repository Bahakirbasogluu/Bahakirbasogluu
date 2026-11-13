# Baha Kırbaşoğlu

AI Engineer at [PEAKUP](https://peakup.org), Türkiye's first and only Microsoft Frontier Partner, and MSc candidate in Computer Engineering at Istanbul Technical University.

I build agentic systems for enterprise clients in banking, energy, logistics and manufacturing: multi-agent orchestration, document pipelines and the tool and review layers around them. I take them from scoping to production and handover. Alongside delivery I teach: university AI courses as an adjunct instructor, and corporate AI training in Turkish and English.

## Client work

Client code lives in private repositories. These are the engagements I can describe.

**Nexent Bank (banking).** Three systems for a Swiss bank.

- *KYC onboarding assistant*, built with Microsoft Agent Framework on Azure AI Foundry behind a FastAPI and React application. A code-owned phase machine takes the relationship manager through the eligibility workbook in batches. For each batch the agent proposes the answers with an evidence class, a confidence and the source documents; the manager confirms or corrects; the confirmed answers are then written into the bank's own workbook in one guarded pass with an audit sheet. It replaces a process that took 2 to 3 weeks per client.
- *Credit risk platform.* Workflows are data: published definitions are compiled into a LangGraph graph in which evidence, financial and policy analysts, a researcher, a synthesizer and a quality reviewer exchange results through typed ports, with bounded fan-out, a bounded review loop and a human interrupt for four-eyes approval. A run pins the version of every agent and workflow it uses and resumes from Postgres checkpoints; work is dispatched through Azure Service Bus to workers on Container Apps.
- *News-watch agent*, live since August 2026. Every hour it scans the press for the companies on the bank's watch-list and sends one deduplicated digest, or nothing when there is nothing new. The model only judges articles that were already fetched and must quote its evidence. In its measured week it did not miss a scheduled hour and its deterministic filters removed 92% of 4,373 candidate articles; a load test scanned 100 watch-list entries in 80 seconds. The same engine is exposed to Copilot Studio as an MCP server.

**Enerjisa (energy).** Document-processing service for 15 document types, among them notary and legal fees, customs and import documents, insurance policies and utility bills. Each document goes through OCR, classification, type-specific extraction with structured outputs, deterministic validation and mapping to SAP-ready records, which the client's RPA posts to SAP, so that the accounting team reviews output instead of keying in data.

**CEVA Logistics (logistics).** Several systems in production in the logistics operation.

- *E-mail-to-order agent.* It reads free-form shipment requests, extracts the order fields, identifies the customer from the tax number and sender, replies with the details that are missing and relays the quote from the pricing system; it does the work of one full-time coordinator, about 8 hours a day.
- *Trip-document OCR pipeline.* It processes 110,000 to 120,000 documents a month with 19 extraction templates, 4 for general document types and 15 customer-specific, each with its own Pydantic schema, on Azure AI Document Intelligence and Azure OpenAI, running as containerised Azure Functions.
- *WhatsApp agents* built as LangGraph state machines. One verifies the customer and collects a shipment request through an order sub-graph, then relays the quote. The other routes customer-service requests through a dispatcher to step-by-step sub-agents that call the transport system's API.

**SASA Polyester (manufacturing).** WhatsApp agent that answers business questions in natural language by querying Power BI directly, so users get reporting figures without opening a dashboard.

**Flormar (cosmetics).** Corporate knowledge assistant on Copilot Studio over 12 SharePoint sources and about 136 documents, mostly HR. It routes each question to the right source, applies date rules to answer from the current version of a document, and hands sensitive topics to HR.

**A hospital group (healthcare).** Proof of concept for a permission-aware RAG assistant embedded in the intranet. Access groups are stamped on every chunk at indexing time and every query carries a security filter, so the model only ever receives documents the signed-in user may see; answers cite their sources. FastAPI, a React widget, Azure AI Search with hybrid retrieval and Azure AI Foundry.

**Kansai Altan (paints).** Containerised three internal business applications for Azure App Service with GitHub Actions pipelines, and wrote the engineering standards they now share: naming, CI/CD and branching.

**PEAKUP (internal).** A sector-neutral case-agent platform that generalises the credit risk work: versioned agents and workflows, gated MCP tool connections, golden-case evaluations that block a release on regression, and sector packs for banking, logistics and pharma. It is designed to be installed in each customer's own tenant.

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
| [agent-workflow-orchestrator](https://github.com/Bahakirbasogluu/agent-workflow-orchestrator) | Multi-agent workflows as data: published definitions compiled to a LangGraph graph, with typed ports between agents, human review as a durable interrupt, pinned versions and golden-case evaluation. |
| [news-watch-agent](https://github.com/Bahakirbasogluu/news-watch-agent) | News-watch agent that scans the press for a watch-list and sends one deduplicated digest: evidence-checked matching, database-enforced deduplication, self-healing delivery and an MCP bridge for other orchestrators. |
| [workbook-review-agent](https://github.com/Bahakirbasogluu/workbook-review-agent) | Agent that pre-fills a review workbook from evidence documents, batch by batch, with a person confirming every answer and a guarded write into the Excel template. |
| [permission-aware-rag](https://github.com/Bahakirbasogluu/permission-aware-rag) | RAG assistant for documents not everyone may read: access groups on every chunk, a security filter on every query and an evaluation that counts leaks. |
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

**Agents and orchestration:** LangGraph, Microsoft Agent Framework, Copilot Studio, Azure AI Foundry, Azure OpenAI, MCP servers and tool gating, human-in-the-loop review, RAG with access control, golden-case evaluation.

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

[Website](https://bahakirbasogluu.github.io) · [LinkedIn](https://www.linkedin.com/in/bahakirbasoglu) · [Medium](https://medium.com/@bahakirbashov) · [Kaggle](https://www.kaggle.com/bahakirbasoglu)

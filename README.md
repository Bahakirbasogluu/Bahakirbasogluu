# Baha Kırbaşoğlu

AI Engineer at [PEAKUP](https://peakup.org), Türkiye's first and only Microsoft Frontier Partner, and MSc candidate in Computer Engineering at Istanbul Technical University.

I build LLM-agent and document-intelligence systems for enterprise clients in banking, energy, logistics and manufacturing, and take them from scoping to production and handover. Alongside delivery I teach: university AI courses as an adjunct instructor, and corporate AI training in Turkish and English.

## Client work

Client code lives in private repositories. These are the engagements I can describe.

| Client | Sector | What I built | Outcome |
| --- | --- | --- | --- |
| Nexent Bank | Banking | KYC onboarding agent on Copilot Studio and Azure AI Foundry. It researches internal policy and completes the eligibility workbook from the documents a client uploads. The same pattern was then applied to credit risk analysis. | Replaced a process that took 2 to 3 weeks per client. Now the relationship managers' standard onboarding workflow. |
| Enerjisa | Energy | Document-processing pipeline that reads 26 document types (invoices, notarial deeds, insurance policies and others) and posts the extracted data to SAP through a custom MCP server. | The accounting team's standard workflow. Staff review output instead of keying in data. |
| CEVA Logistics | Logistics | E-mail-to-order agent that reads free-form shipment requests, extracts order fields against Pydantic schemas, matches the customer, follows up on missing details and returns the quote. | Does the work of one full-time coordinator (about 8 hours a day). The role moved to review. |
| CEVA Logistics | Logistics | Generative-AI OCR pipeline for trip documents across 19 customer-specific templates, on Azure AI Document Intelligence and Azure OpenAI, deployed as serverless Azure Functions through Azure DevOps. | Processes about 120,000 documents a month. |
| SASA Polyester | Manufacturing | WhatsApp agent that answers business questions in natural language by querying Power BI directly. | Users get reporting figures without opening a dashboard. |
| ZF Friedrichshafen | Automotive | Anomaly detection models for manufacturing quality processes, with SHAP and LIME layers that show engineers why a part was flagged. Delivered while at NTT DATA Business Solutions. | 98 to 99% accuracy on live production data, maintained through continuous retraining. |

At PEAKUP I also designed an internal multi-agent system for technical documentation support (classification, summarization, retrieval).

## Teaching and training

**Corporate AI training.** More than 20 days of in-person training on AI agents and Microsoft Copilot Studio for Eczacıbaşı (7 days), KPMG (6), Petroyağ (4) and Hedef Filo (3), plus online programmes for MetLife, TAV and Enerjisa. Sessions run in Turkish or English and are adapted to the audience's sector and departments.

| Programme | Audience | Content |
| --- | --- | --- |
| AI 101 | All employees, half or full day | How generative AI works, what it can and cannot do, prompting, responsible use, department scenarios |
| Microsoft 365 Copilot | Business departments | Copilot in daily work by department: finance, HR, sales, operations, legal, IT |
| Copilot Studio and agent building | Power users and IT | Designing, grounding and publishing agents; hands-on labs with test questions and a prompt-injection demo |
| Technical track | Developers | Azure AI services and AI-assisted development (vibe coding) |

**University teaching.** Adjunct instructor in PEAKUP's Sektör Kampüste programme since 2025, now in its third semester. I teach AI courses at Süleyman Demirel University, Okan University and Kocaeli Health and Technology University: syllabus and exam design, lectures, student projects and grading.

## Research

MSc thesis at Istanbul Technical University: uncertainty-aware, explainable whole-body PET/CT lesion segmentation with a dual-channel nnU-Net.

**Publication.** "Small-Lesion Detection in Whole-Body FDG PET/CT: A Lesion-Level Audit of Training and Post-Processing Trade-offs", first author, accepted at ISMSIT 2026.

## Repositories

| Project | What it is |
| --- | --- |
| [Fraud-Detection](https://github.com/Bahakirbasogluu/Fraud-Detection) | One-class anomaly detectors (OCSVM, GMM, Isolation Forest, LOF) and score ensembles (voting, stacking) for fraud detection on credit card and Medicare data. |
| [Fraud-Detection-GT](https://github.com/Bahakirbasogluu/Fraud-Detection-GT) | The graph-based companion study on the same datasets: centrality and community analysis, spectral methods, and GNNs (GCN, GraphSAGE, GAT, DOMINANT). |
| [IMPBA](https://github.com/Bahakirbasogluu/IMPBA) | Image inpainting for object removal with two U-Net variants, comparing MSE and VGG19 perceptual loss; evaluated with PSNR, SSIM and LPIPS. |
| [docgen_data](https://github.com/Bahakirbasogluu/docgen_data) | Turkish and English technical-support dialogue dataset (341 samples) for issue classification, title generation, sentiment analysis and summarization. |
| [smart-fridge](https://github.com/canatess/smart-fridge) | Undergraduate graduation project: estimating the freshness of produce from visible spoilage. Team project. |

The older repositories on this profile are coursework from my undergraduate years at Hacettepe University.

## Toolbox

- **LLM and agentic AI:** Azure OpenAI, Microsoft Copilot Studio, Azure AI Foundry, LangChain and LangGraph, custom MCP servers, RAG, vector databases, multi-agent orchestration
- **ML, vision and explainability:** PyTorch, TensorFlow, scikit-learn, Hugging Face, LoRA fine-tuning, nnU-Net, YOLO, OpenCV, Azure AI Document Intelligence, SHAP, LIME, uncertainty quantification
- **Cloud and MLOps:** Azure Machine Learning, Azure Functions, Azure AI Search, Azure DevOps, Docker, FastAPI, Redis, Power Platform
- **Languages and data:** Python, SQL, PostgreSQL, Pandas, NumPy, Pydantic

## Experience

- **AI Engineer, PEAKUP** (Aug 2025 to present). End-to-end client AI engagements: scoping, build, production rollout, and handover with runbooks, architecture documentation and team training.
- **AI Engineer, ONO Teknoloji** (May to Aug 2025). Demand forecasting and multi-agent chatbot solutions, including SQL data modelling from raw source systems.
- **Data Scientist, NTT DATA Business Solutions** (Jun 2024 to May 2025). Document translation and chatbot solutions on Azure AI services for Mercedes-Benz Türk, Pegasus and KoçZer, with deployment automated through Azure Machine Learning and Azure Pipelines.
- **Earlier:** AI engineering intern at Selvi Technology (2023); internships at Turkish Aerospace (2021 to 2022) and Bekaert İzmit Çelik Kord (2022); Microsoft Turkey student programme (2022 to 2023).

## Education and certification

- MSc Computer Engineering, Istanbul Technical University (2025 to January 2027, expected)
- BSc Artificial Intelligence Engineering, Hacettepe University (2019 to 2024)
- Microsoft Certified: Azure AI Engineer Associate
- Languages: Turkish (native), English (professional working proficiency), German (A2)

## Writing and speaking

- Articles on applied AI and agentic systems on [Medium](https://medium.com/@bahakirbashov)
- Guest on the PEAKUP Teknoloji Konuşmaları podcast, on multi-agent systems in enterprise workflows

## Contact

[LinkedIn](https://www.linkedin.com/in/bahakirbasoglu) · [Medium](https://medium.com/@bahakirbashov) · [Kaggle](https://www.kaggle.com/bahakirbasoglu)

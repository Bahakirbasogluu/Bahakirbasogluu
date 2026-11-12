# Baha Kırbaşoğlu

AI Engineer at [PEAKUP](https://peakup.org), Türkiye's first and only Microsoft Frontier Partner, and MSc candidate in Computer Engineering at Istanbul Technical University.

I build LLM-agent and document-intelligence systems for enterprise clients in banking, energy, logistics and manufacturing, and take them from scoping to production and handover. Alongside delivery I teach: university AI courses as an adjunct instructor, and corporate AI training in Turkish and English.

## Client work

Client code lives in private repositories. These are the engagements I can describe.

**Nexent Bank (banking).** KYC onboarding agent on Copilot Studio and Azure AI Foundry. It researches internal policy and completes the eligibility workbook from the documents a client uploads, replacing a process that took 2 to 3 weeks per client. It is now the relationship managers' standard onboarding workflow, and the same pattern was applied to credit risk analysis.

**Enerjisa (energy).** Document-processing pipeline that reads 26 document types, including invoices, notarial deeds and insurance policies, and posts the extracted data to SAP through a custom MCP server. The accounting team now reviews output instead of keying in data.

**CEVA Logistics (logistics).** Two systems, both now standard in the logistics operations unit. An e-mail-to-order agent reads free-form shipment requests, extracts order fields against Pydantic schemas, matches the customer, follows up on missing details and returns the quote; it does the work of one full-time coordinator, about 8 hours a day. A generative-AI OCR pipeline processes about 120,000 trip documents a month across 19 customer-specific templates, on Azure AI Document Intelligence and Azure OpenAI, deployed as serverless Azure Functions.

**SASA Polyester (manufacturing).** WhatsApp agent that answers business questions in natural language by querying Power BI directly, so users get reporting figures without opening a dashboard.

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

**LLM and agents:** Azure OpenAI, Copilot Studio, Azure AI Foundry, LangChain and LangGraph, custom MCP servers, RAG, multi-agent orchestration.

**ML and cloud:** PyTorch, scikit-learn, Hugging Face, nnU-Net, Azure AI Document Intelligence, SHAP and LIME, Azure Functions, Azure Machine Learning, Azure DevOps, Docker, FastAPI.

## Background

- MSc Computer Engineering, Istanbul Technical University (2025 to January 2027, expected)
- BSc Artificial Intelligence Engineering, Hacettepe University (2019 to 2024)
- Microsoft Certified: Azure AI Engineer Associate
- Before PEAKUP: Data Scientist at NTT DATA Business Solutions, AI Engineer at ONO Teknoloji

## Writing and speaking

- Articles on applied AI and agentic systems on [Medium](https://medium.com/@bahakirbashov)
- Guest on the PEAKUP Teknoloji Konuşmaları podcast, on multi-agent systems in enterprise workflows

## Contact

[LinkedIn](https://www.linkedin.com/in/bahakirbasoglu) · [Medium](https://medium.com/@bahakirbashov) · [Kaggle](https://www.kaggle.com/bahakirbasoglu)

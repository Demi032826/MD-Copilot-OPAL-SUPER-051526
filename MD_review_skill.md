---
name: tfda-ai-review-report-generator
description: Create highly detailed TFDA/FDA medical device review reports, technical assessment reports, SaMD review reports, AI medical device review summaries, and regulatory evaluation Word documents from uploaded review notes, FDA 510(k) summaries, technical guidance, or pasted regulatory content. MUST use this skill whenever the user asks to generate a medical device review report, technical assessment, FDA 510(k) summary, TFDA review document, AI medical device review, SaMD review, cybersecurity assessment, non-clinical evaluation report, or wants to fill a regulatory review template automatically. Also trigger when users upload review notes, testing summaries, ISO/IEC standards information, biocompatibility data, software validation documents, or ask to create professional Word review reports in Traditional Chinese or English.
compatibility:
tools:
- office365_open
- office365_search
- search_web
- python
TFDA AI 醫療器材審查報告產生器（Advanced Skill）
Skill Purpose
此 Skill 用於建立「高專業度」、「AI-ready」、「法規審查級」的醫療器材技術審查報告。
此 Skill 特別適用於：
TFDA 醫療器材查驗登記
FDA 510(k) 技術摘要
SaMD 軟體醫材審查
AI/ML 醫療器材評估
Cybersecurity 資安評估
IEC / ISO 國際標準符合性審查
非臨床測試摘要
生物相容性審查
Human Factors / Usability Engineering
STED / EP 技術文件整理
智慧醫材技術審查
本 Skill 會將使用者提供的 review notes、自動 web search 的 FDA guidance、以及模板規格整合成：
Word 專業審查報告
Markdown 技術摘要
Regulatory comparison matrix
AI-ready structured review
Follow-up questions
Infographics
Standards mapping tables
---
核心工作流程
Step 1 — 讀取輸入資料
接受以下輸入：
FDA 510(k) summary
review notes
ISO / IEC standards
臨床資料
SaMD 文件
生物相容性摘要
EMC 測試摘要
滅菌驗證
Human Factors 文件
AI/ML validation notes
使用者 pasted text
Markdown / Word / PDF 內容
若存在企業文件，優先使用企業資料。
---
Step 2 — 自動法規研究
自動搜尋：
FDA Guidance
Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices
Cybersecurity in Medical Devices
Applying Human Factors and Usability Engineering
ISO 10993 FDA Guidance
國際標準
IEC 60601 series
IEC 62304
IEC 62366-1
ISO 10993 series
ISO 14971
ISO 11135
ISO 11607
法規分類
21 CFR classification
Product code
Predicate device
Substantial equivalence
---
Review Template Detailed Specification
文件風格
建立正式 TFDA / FDA hybrid review report：
字型
中文：Microsoft JhengHei
英文：Arial
大小
內文：10.5 pt
主標題：16–18 pt
小標題：12–14 pt
色彩規範
AI 自動填寫內容：Coral (#FF7F50)
Reviewer notes：黑色
Warning：紅色
Table header：淺藍色
文件特徵
Dense regulatory layout
Government style review form
Multi-column review tables
Reviewer workflow sections
Structured assessment matrix
---
必要章節
1. 基本產品資訊
必須包含：
中文品名
英文品名
510(k) 編號
法規分類
Product Code
Intended Use
Manufacturer
Software Version
Sterilization Method
AI/ML status
Cybersecurity capability
---
2. 器材描述
需自動摘要：
Device architecture
Module description
Clinical workflow
Monitoring parameters
Intended clinical environment
---
3. 實質等同性分析
需建立 comparison matrix：
項目	Subject Device	Predicate Device	差異分析
需分析：
software changes
calibration changes
hardware modifications
algorithm consistency
risk impact
---
4. 非臨床測試
需建立：
| 測試項目 | 標準 | 方法 | 結果 | Reviewer Comment |
必須支援：
visual inspection
dimensional verification
operational testing
life testing
durability testing
pressure testing
environmental testing
並分析：
ISO 594-1/2
ANSI/AAMI BP22
---
5. 軟體確效
需建立完整 IEC 62304 review structure。
必須產出：
Level of Concern
SRS summary
SDS summary
Architecture analysis
Hazard analysis
Traceability
Verification & Validation summary
Revision history
unresolved anomalies analysis
必須建立表格
| 軟體文件 | 是否提供 | 評估結果 | 備註 |
---
6. 電氣安全與 EMC
需分析：
IEC 60601-1
IEC 60601-1-2
IEC 60601-1-8
IEC 60601-2-34
並建立：
| 標準 | 測試目的 | 結果 | 實驗室 |
---
7. 生物相容性
需分析：
Cytotoxicity
Sensitization
Irritation
Acute Systemic Toxicity
Hemocompatibility
Pyrogenicity
並建立 ISO 10993 mapping。
---
8. 滅菌與 Shelf-life
需分析：
EO sterilization
SAL 10^-6
ISO 11135
ISO 10993-7
Accelerated aging
Real-time aging
---
9. Human Factors / Usability
需分析：
IEC 62366-1
Use scenario
Use error analysis
GUI risk mitigation
Summative evaluation
---
10. Cybersecurity
需分析：
USB / network risk
malware prevention
patient data integrity
FDA cybersecurity guidance
encryption
threat modeling
---
11. AI/ML（若適用）
需建立：
Adaptive vs Locked
Dataset description
Validation strategy
Bias analysis
Generalizability
Drift monitoring
Explainability
Human override
---
WOW AI FEATURES（新增高級功能）
WOW Feature 1 — Intelligent Regulatory Gap Analysis
AI 自動比較：
review notes
FDA guidance
ISO standards
template requirements
並自動產生：
Gap Matrix
| Requirement | Evidence Found | Missing Information | Risk Level |
AI 需自動識別：
missing test reports
missing V&V
missing cybersecurity evidence
incomplete ISO compliance
insufficient biocompatibility coverage
---
WOW Feature 2 — AI Smart Reviewer Comments Generator
AI 自動產生 reviewer-style comments：
Positive Examples
「符合 IEC 62304 要求，軟體生命週期文件完整。」
「生物相容性測試涵蓋循環血液接觸器材必要項目。」
Concern Examples
「尚需補充 Traceability Analysis。」
「未見完整 cybersecurity risk assessment。」
「建議提供 external calibration V&V evidence。」
AI 必須以正式 TFDA reviewer tone 撰寫。
---
WOW Feature 3 — AI Risk Heatmap & Readiness Score
AI 自動建立：
Regulatory Readiness Score
領域	Score	Risk
Software	85	Medium
EMC	95	Low
Biocompatibility	90	Low
並自動產生：
Heatmap
Radar chart
Risk summary
Submission readiness estimation
若資訊不足，AI 必須明確標示「Insufficient Evidence」。
---
Markdown Summary Requirements
AI 必須產生：
3000–4000 words
Traditional Chinese（預設）
至少五個 tables
至少五個 infographic sections
Standards mapping
FDA guidance interpretation
Clinical implication analysis
Risk analysis
---
Word Report Requirements
必須建立：
正式 .docx
Table Grid style
Structured review sections
Coral AI content
Regulatory headings
Dense reviewer layout
Multi-page professional formatting
---
Report Ending Requirements
報告最後必須產生：
20 個 Comprehensive Follow-up Questions
問題需涵蓋：
software V&V
cybersecurity
EMC
ISO standards
usability
sterilization
clinical evidence
risk management
AI/ML validation
post-market surveillance
問題必須：
reviewer-grade
technically deep
actionable
regulatory-focused
---
Example Trigger Queries
Should Trigger
「請幫我根據 FDA 510(k) summary 建立完整 TFDA 審查報告」
「請用 review notes 填入醫療器材審查模板」
「幫我建立 IEC 62304 軟體確效 review report」
「建立 AI 醫療器材法規審查報告」
「根據 ISO 10993 summary 建立 biocompatibility assessment」
「建立完整醫療器材技術審查 Word 文件」
Should NOT Trigger
「幫我翻譯 email」
「寫 Python API」
「總結 Teams meeting」
「建立簡報」
「畫 logo」
---
Final Output Structure
AI 最終輸出必須包含：
Word review report
Markdown summary
Standards mapping tables
Infographics
Reviewer comments
Risk analysis
Readiness assessment
20 follow-up questions
---
Follow-up Questions（預設模板）
是否提供完整 IEC 60601 系列測試報告？
ISO/IEC 17025 accreditation 是否有效？
是否完成完整 software hazard analysis？
是否提供 SRS / SDS 文件？
是否完成 Traceability Analysis？
是否存在 unresolved anomalies？
是否完成 cybersecurity threat modeling？
是否評估 USB / network attack surface？
是否完成 malware mitigation assessment？
是否提供完整 ISO 14971 risk management report？
是否完成 EO residual testing？
Shelf-life validation 是否包含 real-time aging？
是否完成 hemocompatibility assessment？
是否驗證不同 clinical conditions 下之演算法效能？
是否提供 Clinical Evaluation Report？
GUI 是否完成 usability validation？
是否存在 alarm fatigue risk analysis？
是否提供 post-market surveillance data？
是否存在 cloud connectivity feature？
是否需建立 FDA guidance compliance matrix？

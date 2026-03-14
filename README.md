# Sequential Interventions and AI Adoption: An 18-Month Longitudinal Case Study
 
**Paper prepared for the [Wharton Human-AI Research (WHAIR) Conference](https://whair.wharton.upenn.edu/) — *AI and the Future of Work*, May 20–21, 2026**
 
**Author:** Sara Maldon · Head of Business Automation & AI, [Make](https://make.com)
 
---
 
## Overview
 
This repository contains the full paper, reproducible analysis, and anonymised dataset for a longitudinal case study documenting enterprise-wide AI adoption at a 349-person SaaS company over 18 months.
 
The study examines three sequential interventions — voluntary tool access, structural enablement with departmental facilitators, and mandatory accountability tied to performance evaluations — and their effect on employee-level AI adoption rates. Key findings:
 
- **Voluntary access** → 2.6% mean monthly adoption (Rogers' innovator segment)
- **Structural enablement** → 8.1% mean monthly adoption
- **Mandatory accountability** → 32.1% mean monthly adoption (4.0× increase), peak of 59.6%
- **Post-mandate retention** → 26.1%, 3× above pre-mandate ceiling
- **Cumulative reach** → 96.3% of eligible employees built at least one AI-enabled workflow
 
Counterfactual modelling suggests majority adoption would not have occurred until ~January 2028 without the mandate — 29 months later than observed.
 
## Repository Contents
 
| File | Description |
|------|-------------|
| `Sequential_Interventions_AI_Adoption_Paper.docx` | Full paper (Word format) |
| `miriwa_analysis.ipynb` | Jupyter notebook — all statistical analysis and figure generation |
| `AI_Scenarios_Dataset_2026_Anonymized.csv` | Anonymised dataset (8,802 workflow records, 349 employees, 8 departments) |
| `fig1–fig6*.png` | Pre-rendered figures used in the paper |
| `Appendix_A_Figures.docx` | Appendix with all figures and captions |
| `Section_3_Findings.docx` | Standalone findings section |
 
## Dataset Schema
 
The CSV contains **8,802 rows** (one per automation workflow) with the following columns:
 
| Column | Type | Description |
|--------|------|-------------|
| `ID_scenario` | int | Unique workflow identifier |
| `CreatedBy` | string | Anonymised employee ID (e.g. `EMPLOYEE_01`) |
| `Department` | string | Organisational unit (8 departments) |
| `Created` | date | Workflow creation date (DD/MM/YYYY) |
| `LastEdit` | date | Last modification date |
| `isActive` | binary | Whether the workflow is currently active |
| `isAiUsed` | binary | Whether the workflow uses AI capabilities |
| `isAiAgentUsed` | binary | Whether the workflow uses AI agents |
 
## Reproducing the Analysis
 
```bash
# Clone the repo
git clone https://github.com/<your-org>/whair-sequential-interventions.git
cd whair-sequential-interventions
 
# Install dependencies (Python 3.10+)
pip install pandas matplotlib seaborn scipy numpy jupyter
 
# Run the notebook
jupyter notebook miriwa_analysis.ipynb
```
 
## Citation
 
```bibtex
@inproceedings{maldon2026sequential,
  title     = {Sequential Interventions and their Role in {AI} Adoption: An 18-Month Longitudinal Case Study in a 349-Person {SaaS} Company},
  author    = {Maldon, Sara},
  booktitle = {Wharton Human-AI Research (WHAIR) Conference: AI and the Future of Work},
  year      = {2026},
  month     = {May}
}
```
 
## Keywords
 
`enterprise AI adoption` · `organizational change` · `mandate effects` · `employee-level metrics` · `longitudinal case study` · `workflows`
 
## License
 
This dataset and analysis are shared for academic and research purposes. Please cite the paper if you use any materials from this repository.
 
---
 
*Questions or collaboration inquiries → reach out via [LinkedIn]([https://linkedin.com/in/saramaldon]) or open an issue.*
 

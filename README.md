# Youth Scouting Analytics – Manchester City FC 

_FIFA 23 Talent-Pipeline Dashboard in Tableau & Power BI_

[[Tableau Public](https://public.tableau.com/app/profile/bimal.bimal/viz/youthscouting_mancity_tableu/Dashboard2?publish=yes )


[[Power BI] (https://app.powerbi.com/view?r=eyJrIjoiOGQ1MTFmMTctNzI2MC00OThhLTkwYjAtNWEyYzNkODVhMzBjIiwidCI6IjVkMGFhNmVhLTY2MjAtNDg2My05ZTIxLTllY2IxNDAyMjJiYyIsImMiOjh9)

## 1  Project Overview
A dual-build data-visualisation project that explores the *_FIFA 23 Complete Player Dataset*_
(57 010 players × 1 144 clubs) through the lens of youth scouting for Manchester City FC.

*Two fully-featured, functionally-equivalent dashboards were created—one in
**Tableau**  and one in **Power BI**—to answer three scouting questions:*



CEO / Owner | What is the _current & potential financial value_ of our talent pipeline? | Value-for-Money scatter · Global Value Academies bar 
Head of Youth Recruitment | Which _clubs, countries & age-bands_ produce the best prospects? | Bubble map · Age–Growth curve · interactive slicers |
First-Team Coach| Who are the _Top-5 high-ceiling players_ per position? | Dense-rank Top-N bar · parameter-driven VfM scatter |

---

## 2  Data Source
> “FIFA 23 Complete Player Dataset”**  
> Kaggle | last updated 2023-10-27  

Four raw CSVs (men/women players & teams) were cleaned in **Power Query**  
and exported to `Players_all.csv` & `Teams_all.csv`.

## 3  Key Features
* Automated **Power Query** cleaning (duplicate PlayerID/TeamID removal, NULL fixes,  
  negative value correction).  
* Tableau **FIXED LOD** vs Power BI **DAX** (`RankX`, `GENERATESERIES`, `AVERAGEX`).  
* Top-N parameter (1-5) driving player list and VfM scatter in real time.  
* Country-action drill-down: map click filters the other three visuals.  
* Dynamic titles (`Country Label | Top N | Age Band | Gender | Position`) in both tools.  
* Branded in Manchester-City sky-blue (#6CABDD) with club crest watermark.

---

## 4  Repository Structure
Main Root
├─ Dashboards/ 
  ├─📊 Youth_Scouting_PowerBI.pbix   – interactive BI report
  ├─📊 Youth_Scouting_Tableau.twbx   – Tableau workbook (packaged)
├─📂 Reports/
  ├─Youth_Scouting_Critical_Report.pdf
  ├─Youth_Scouting_Appendix.pdf   – full DAX / LOD equations
├─📂 Data/
│   ├─ Players_clean.csv           – 57 010 rows
│   └─ Teams_clean.csv             – 1 144 rows
└─README.md                        – you are here

## 5  Quick Start
### View the dashboards
1. **Tableau:** click the badge at the top or open `Youth_Scouting_Tableau.twbx`  
   in Tableau Desktop / Reader.  
2. **Power BI:** click the badge or open `Youth_Scouting_PowerBI.pbix` in  
   Power BI Desktop (Oct-2023 or later).

Built as CA-2 submission for TU Dublin MSc Computing (Data Analytics):
module Data Visualisation & Storytelling, Semester 2 2025.

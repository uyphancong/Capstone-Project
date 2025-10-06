# 🎯 Deakin × World Vision Australia — Bounceback Campaign Analysis

## 📘 Overview
This project was conducted as part of the MIS779 *Decision Analytics in Practice* unit at Deakin University, in collaboration with **World Vision Australia (WVA)**.  
The analysis focuses on optimising WVA’s **Bounceback Campaign**, which aims to re-engage lapsed child sponsorship donors through personalised, multi-channel communications.

Our team applied both **diagnostic** and **predictive analytics** to uncover data-driven insights that improve donor engagement, campaign efficiency, and long-term return on investment (ROI).

---

## 🎯 Objectives
- Evaluate supporter engagement patterns and donation behaviours.
- Optimise the **journey** (timing and frequency of contact) for higher response rates.
- Align **targeting** strategies with donor communication preferences.
- Personalise **donation asks** to increase average contribution and campaign ROI.

---

## 🧩 Methodology

### 1. Data Preparation
- Merged datasets from communications, donations, demographics, and engagement.
- Aggregated at the supporter level (Deakin_SupporterID).
- Cleaned and standardised variables; engineered new features:
  - Number of Contacts  
  - Average Contact Interval  
  - Total Donated  
  - Portal Engagement Flags  
  - Days Since Last Contact  

### 2. Analytical Framework
| Pillar | Analytical Approach | Key Tools |
|--------|---------------------|------------|
| **Journey** | Event & timing analysis; Random Forest classification for donation likelihood | Python (Pandas, Scikit-learn), Tableau |
| **Targeting** | Behavioural segmentation & channel alignment | Tableau, Power BI |
| **Ask** | Gap analysis & Random Forest regression for optimal ask prediction | Python, SHAP |

---

## 📊 Key Findings

### 🕒 Journey – Optimise Timing & Contact Volume
- Donor response **peaked at the 2nd contact**; declines after excessive outreach.  
- **12–14 days** is the optimal interval between contacts to maximise engagement.  
- Random Forest classification achieved **93% precision**, enabling accurate supporter segmentation (High → Low tiers).

### 🎯 Targeting – Align Channels with Behaviour
- Many digitally active supporters are still receiving offline communications.  
- Donors **under 50** prefer online channels, while **60+** donors respond better to offline.  
- Aligning stream assignments with actual digital behaviour improves engagement and cost-efficiency.

###  Ask – Personalise Suggested Donation Amounts
- **52.8%** of donors gave **below** the suggested amount — indicating misaligned asks.  
- A Random Forest regression model (R² = 0.65, MAE = \$3.13) predicts optimal donation requests.  
- Key predictors: prior ask amount, contact frequency, tenure, number of children sponsored.

---

##  Recommendations Summary
| Area | Recommendation |
|-------|----------------|
| **Journey** | Limit to 2 contacts per campaign (12–14 day interval); focus on high-likelihood supporters. |
| **Targeting** | Use behavioural signals (portal activity, email engagement) to assign channels dynamically. |
| **Ask** | Implement model-driven ask suggestions tailored to donor history and engagement. |

---

##  Tools & Technologies
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SHAP)  
- **Tableau / Power BI** for visualisation  
- **RapidMiner** for data mining and automation  
- **Microsoft Excel** for data aggregation and validation  

---

##  Team Members
| Name | Student ID |
|------|-------------|
| Ha Cam Nguyen | s223546667 |
| Uy Cong Phan | s223626353 |
| Andrea Aponsu | s224072494 |
| Thilini Munasinghe | s223733272 |
| Siteng Zhou | s224803109 |
| Adithya Anuradhanayake | s224242915 |

---

##  Unit Information
- **Unit:** MIS779 – Decision Analytics in Practice  
- **Trimester:** T2, 2024  
- **Institution:** Deakin University, Australia  
- **Client:** World Vision Australia (Analytics, Insights & Marketing Technology)

---

##  License
This project is released under the **MIT License**.  
Data used is anonymised and solely for academic purposes.

---

##  Contact
**Contributor:** [Uy Phan (Phan Cong Uy)](https://www.linkedin.com/in/phan-cong-uy-b0ab60124/)  
📧 Email: s223626353@deakin.edu.au  

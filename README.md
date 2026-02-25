# PCAF-Projects
 

Financed & Facilitated Emissions Tool

Project Overview

This project simulates a $616B global bank portfolio to analyze carbon exposure across both lending and capital markets activities. Using PCAF (Partnership for Carbon Accounting Financials) standards, I developed an end-to-end tool to quantify and disclose "On-Balance Sheet" emissions (Lending/Investments) and "Off-Balance Sheet" emissions (Underwriting/Facilitation).

Key Features

1. Dual-Scope GHG Accounting:
  - Financed Emissions: Analysis of $616B in funded loans using WACI (tCO2​e/$1M) and absolute footprinting.
  - Facilitated Emissions: (Upcoming) Calculation of emissions associated with debt and equity underwriting, applying the PCAF 33% weighting factor for capital market activities.

2. Carbon Overhang & Risk Delta: Identifies "Shadow Footprints" by calculating the gap between realized and committed capital, highlighting sectors like Mortgages (114% Delta) as high-volatility risks.

3. Data Integrity Engine: Implements PCAF Data Quality Scores (1-5) to provide a "Confidence Score" for all reported figures.

4. Dynamic Executive Dashboard: Automated visuals tracking sector-wise intensity, capital utilization, and transition risk hotspots.

Tool Architecture

    
    02_Firm_Parameters: Master logic, sector mapping, and Facilitation weighting factors.

    03_Entity_Master: Source of truth for total bank exposure and underwriting deal flow.

    04_Legal_Entity_Data: Client-level GHG data and PCAF data quality management.

    05_PCAF_Engine: Automated attribution math for both funded and facilitated emissions.

    01_Executive_Summary: Integrated view of Total Portfolio WACI and "Off-Balance Sheet" climate risk.

    06_Technical_Appendix: Proxy-based estimation calcualations

Methodology & Assumptions

Normalization: All WACI metrics are reported in tCO2​e/$1M to align with international financial reporting standards.

Prudential Approach: The tool assumes a 100% drawdown scenario for committed lines to stress-test the bank's Net Zero alignment.

Audit Trail: Every estimation relies on the Technical Appendix, ensuring that proxy-based "Score 4/5" data is transparently disclosed.

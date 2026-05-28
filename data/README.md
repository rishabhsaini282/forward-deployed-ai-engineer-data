# FDE Salary Data Dictionary

This directory contains the machine-readable total compensation data for Forward-Deployed AI Engineers (FDEs) updated for May 2026.

## Data Methodology
*   **Sources:** Aggregated from public job postings (OpenAI, Anthropic, Palantir), verified levels.fyi offer data (Jan-Apr 2026), and regional TeamLease Digital GCC reports.
*   **Base vs Equity:** Standard base salaries face natural corporate compression. Annualized equity is the primary vehicle for wealth generation above mid-level. By the Staff level, equity packages routinely exceed base cash.
*   **Remote Adjustments:** Fully remote configurations carry an immediate 10–15% structural salary markdown compared to on-site equivalents.
*   **India GCC Context:** Senior FDE professionals within Global Capability Centers (Bengaluru, Hyderabad, Pune) pull total compensation packages ranging from ₹65L to ₹2.2Cr.

## Column Definitions
*   `Level`: Industry-standard engineering tier.
*   `Years_Experience`: Typical baseline production experience required.
*   `Base_Min` / `Base_Max`: Cash base salary range (USD).
*   `Equity_Annual_Min` / `Equity_Annual_Max`: Annualized stock options, RSUs, or PPUs tied to preferred-round valuations.
*   `Sign_On_Min` / `Sign_On_Max`: First-year variable cash signing bonuses.
*   `Total_Comp_Min` / `Total_Comp_Max`: Cumulative first-year earnings.

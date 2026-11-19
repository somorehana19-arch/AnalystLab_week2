 E-Commerce Business Performance &
Customer Behaviour Analysis
Author: Reyhana Abdikher Programme: AnalystLab Africa Experience Lab Internship — Week
2 (Track 2: Data Science) Dataset: Maven Fuzzy Factory (March 2012 – March 2015)
Project Overview
This repository contains an end-to-end Exploratory Data Analysis (EDA) of three years of
e-commerce operations for Maven Fuzzy Factory. Using Python (Pandas, NumPy, SciPy,
Matplotlib, and Seaborn), the analysis examines website traffic, marketing channel efficiency,
device conversion gaps, product revenue, customer repeat rates, and refund trends across
472,871 sessions and 32,313 completed orders.
Repository Structure
AnalystLab_week2/
├── AnalystLab_Africa_Week2.ipynb # Full Jupyter Notebook (data cleaning, EDA,
statistical tests & charts)
├── .gitignore # Excludes large raw CSV datasets from version control
└── README.md # Project summary, key findings & setup instructions
(Note: Raw CSV files are excluded via .gitignore due to file size. To run the notebook locally,
place the six Maven Fuzzy Factory CSV files in the root folder.)
Key Findings
● Overall Revenue & Conversion: Across 472,871 sessions, the store recorded 32,313
orders (6.83% conversion rate) and $1,938,509.75 in gross revenue ($1,216,139.50
gross margin; 62.74%). Monthly revenue peaked in December 2014 ($144,823.02) during
holiday gifting.
● Desktop vs. Mobile Conversion Gap: Desktop accounts for 69.16% of traffic and
converts at 8.50%, whereas mobile accounts for 30.84% of traffic but converts at only
3.09% (\chi^2 = 4,638.43, p < 0.0001).
● Product & Cross-Sell Performance: The Original Mr. Fuzzy generates 62.47% of total
revenue ($1.21M). Meanwhile, The Hudson River Mini bear acts primarily as an add-on
product (88.42% of its units were sold as cross-sell items), helping lift average order value
from $49.99 in 2012 to $63.80 in 2014.
● Marketing Channel Efficiency: gsearch drives 66.83% of sessions (6.75% conversion),
while direct / organic (7.34%) and bsearch (7.19%) convert strongest. Paid social
(socialbook) converts at half the site average (3.21%).
● Refund Patterns: Total refunds amounted to $85,338.69 (1,731 items; 4.40% of gross
revenue). The Birthday Sugar Panda has the highest structural refund rate (6.04%), while
The Original Mr. Fuzzy experienced a temporary supplier quality spike in August–September 2014 (13.3%–13.8%) before returning to normal.
● Low Repeat Purchase Rate: Out of 31,696 unique paying customers, only 591
(1.86%) placed more than one order, though returning sessions convert 18% higher than
new sessions (7.83% vs. 6.64%).
Business Recommendations
1. Redesign the Mobile Checkout Funnel: Simplifying mobile product pages and checkout
steps to close even half the conversion gap with desktop could generate ~$237,000 in
added revenue from existing traffic.
2. Reallocate Paid Spend from socialbook to Search: Shift budget away from
low-converting socialbook campaigns (3.21%) toward high-intent bsearch and gsearch
keywords.
3. Automate Two-Bear Cart Bundles: Prompt Mr. Fuzzy and Forever Love Bear buyers
with The Hudson River Mini bear at checkout to increase multi-item orders.
4. Audit Quality on The Birthday Sugar Panda: Review supplier stitching and product
descriptions to bring its 6.04% refund rate down toward the rest of the catalog.
5. Launch Post-Purchase Email Retention Flows: Target one-time buyers (98.14% of
customers) with 30- to 90-day lifecycle reminders around birthdays and holidays.
6. Concentrate Ad Bids on Weekday Daytime Hours: Order volume peaks
Monday–Friday between 11:00 AM and 4:00 PM and drops by over 55% on weekends.
How to Run Locally
1. Clone this repository:
git clone https://github.com/somorehana19-arch/AnalystLab_week2.git
cd AnalystLab_week2
2. Install dependencies:
pip install pandas numpy scipy matplotlib seaborn jupyter
3. Place the six dataset files (website_sessions.csv, website_pageviews.csv,
orders_mav.csv, order_items.csv, order_item_refunds.csv, products.csv) in the project
directory and run AnalystLab_Africa_Week2.ipynb

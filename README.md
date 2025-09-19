# Uber Ride Data Analysis: A Deep Dive into Trip Cancellations

### 1. Project Overview

This project analyzes over 6,700 Uber ride requests in a metropolitan area to identify the root causes of trip cancellations and the supply-demand gap. By understanding when and why trips fail, we can provide data-driven recommendations to help Uber improve service reliability, optimize driver allocation, and enhance customer satisfaction.

### 2. Tools & Technologies

-   **Data Cleaning & Analysis:** Python (Pandas, Matplotlib, Seaborn) in a Jupyter Notebook
-   **Interactive Dashboarding:** Tableau
-   **Version Control:** Git & GitHub

### 3. Key Findings & Visualizations

The analysis uncovered a clear narrative of two distinct problem periods driven by location and time.

#### Finding 1: High Demand Peaks in Morning and Evening

The demand for rides is not consistent throughout the day. It peaks during the morning commute (7-9 AM) and again during the evening rush (5-8 PM).

![Demand by Hour](assets/demand_by_hour.png)

#### Finding 2: The Two-Sided Problem: Cancellations vs. Car Shortages

The core issue is a severe supply-demand gap during peak hours, but the *reason* for the gap changes dramatically depending on the time of day.

-   **Morning Rush (City -> Airport):** Characterized by a high number of **driver cancellations**.
-   **Evening Rush (Airport -> City):** Characterized by a severe **shortage of available cars**.

![Status by Hour](assets/status_by_hour.png)

### 4. Interactive Dashboard

An interactive dashboard was created in Tableau to allow for a deeper, more dynamic exploration of these findings. Stakeholders can filter by location and time to see the specific pain points.

[**View the Interactive Dashboard on Tableau Public**](https://YOUR_TABLEAU_PUBLIC_LINK_HERE)

![Dashboard Screenshot](assets/dashboard_screenshot.png)

### 5. Actionable Recommendations

Based on the analysis, the following strategies are recommended:

1.  **Implement a Driver Incentive Program for Airport Pickups:** To address the evening car shortage at the airport, offer drivers a bonus for completing trips originating from the airport between 5 PM and 10 PM. This directly tackles the "No Cars Available" issue.

2.  **Optimize Morning Driver Allocation:** Since morning cancellations from the city are high (likely due to drivers rejecting airport-bound trips), Uber could provide drivers with visibility on their next trip *before* they complete their current one. This would allow a driver heading to the airport to be pre-assigned a return trip, making the initial journey more profitable and less likely to be cancelled.

3.  **Launch a "Pre-Book for Airport" Feature:** For evening airport pickups, allow customers to pre-book their rides. This would give Uber a clearer demand forecast, enabling them to better manage driver supply and reduce the "No Cars Available" rate.

### 6. How to Run This Project

1.  Clone the repository: `git clone https://github.com/YOUR_USERNAME/Uber-Data-Analysis-Project.git`
2.  The raw dataset is located in the `/data` folder.
3.  The complete Python analysis and data cleaning process can be found in the Jupyter Notebook inside the `/notebooks` folder.

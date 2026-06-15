# blood-donation-analytics
# Personal Health Metrics & Blood Donation History Analysis (2017–2026)
A 9-year longitudinal data analysis study of blood donation vitals and operational yields.

## 1. Project Overview
Over the last nine years (2017 to 2026), I logged the health screening data from every blood donation attempt I made. I wanted to throw this history into Python to see what a long-term look at my vitals such as iron levels, blood pressure, and heart rate actually looked like, and figure out the exact patterns behind why I got deferred a few times.

---

## 2. The Raw Data
This dataset tracks 24 donation attempts, including the vital signs taken by the screening staff before each draw:

| Date | Location | Systolic | Diastolic | Hemoglobin | Pulse | Donation Completed |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: |
| 4/4/2017 | Bacon Academy | 132 | 90 | 17.3 | 86 | Yes |
| 11/3/2017 | Bacon Academy | 120 | 74 | 16.9 | 84 | Yes |
| 4/11/2018 | Bacon Academy | 108 | 64 | 18.9 | 60 | Yes |
| 8/1/2018 | Bacon Academy | 122 | 74 | 17.1 | 84 | Yes |
| 4/11/2019 | Bacon Academy | 118 | 80 | 18.8 | 74 | Yes |
| 6/26/2019 | Congregation Ahavath Achim | 120 | 76 | 16.6 | 68 | Yes |
| 8/21/2019 | St. Andrews Catholic Church | 112 | 70 | 17.4 | 78 | Yes |
| 10/16/2019 | Colchester Hayward Fire Dept. | 120 | 80 | 14.8 | 70 | Yes |
| 12/13/2019 | Colchester Federated Church | 110 | 62 | 14.6 | 72 | Yes |
| 2/14/2020 | Colchester Federated Church | 112 | 70 | 13.7 | 70 | Yes |
| 5/18/2020 | CrossFit Playground | 108 | 72 | 14.1 | 72 | Yes |
| 7/15/2020 | William J. Johnston Middle School | 120 | 72 | 12.5 | 60 | No |
| 8/19/2020 | St. Andrews Catholic Church | 122 | 68 | 11.3 | 70 | No |
| 10/20/2020 | Stranger Tides Brewing | 108 | 70 | 13.6 | 72 | Yes |
| 12/18/2020 | St. Andrews Catholic Church | 110 | 70 | 14.4 | 72 | Yes |
| 2/23/2021 | Stranger Tides Brewing | 106 | 82 | 13.5 | 72 | Yes |
| 5/17/2021 | St. Andrews Catholic Church | NaN | NaN | 11.2 | NaN | No |
| 3/29/2022 | St. Joseph's Polish Society | 112 | 70 | 15.3 | 64 | Yes |
| 9/30/2022 | Colchester Hayward Fire Dept. | 116 | 76 | 17.9 | 74 | Yes |
| 2/10/2023 | Colchester Town Hall | 118 | 74 | 16.8 | 74 | Yes |
| 9/11/2023 | St. Andrews Catholic Church | 110 | 70 | 17.1 | 76 | Yes |
| 12/26/2023 | St. Joseph's Polish Society | 104 | 66 | 13.7 | 76 | Yes |
| 8/20/2024 | St. Joseph's Polish Society | 110 | 60 | 16.4 | 80 | Yes |
| 6/8/2026 | Colchester Town Hall | 110 | 71 | 17.1 | 70 | Yes |

---

## 3. Core Insights & Visualizations

### Iron_Trends
My iron levels started out quite high, topping out at 18.9 g/dL in 2018. The most interesting trend is the sudden drop between mid-2020 and mid-2021. You can see exactly where I hit a wall and got deferred three times (marked by the red dots) for dropping below the standard 13.0 g/dL line. After May 2021, my levels bounced back completely and stabilized through 2026.

### Blood_Pressure_Trends
This graph maps my Systolic and Diastolic trends against standard baseline markers (120/80 mmHg), using the shaded gap to highlight my pulse pressure variance over time. My blood pressure has been solid for nearly a decade; my very first reading back in 2017 was the highest at 132/90 mmHg, but the numbers have steadily leveled out, becoming remarkably consistent from 2024 onward.

### Pulse_Rate_Trends
My heart rate has stayed perfectly healthy across the entire timeline, sitting comfortably inside the standard 60-100 bpm resting range (the green band). The data catches a couple of highly efficient, athletic dips down to 60 bpm in 2018 and 2020, and shows a really steady trend hovering between 70 and 76 bpm over the last few years.

### Donation_Center
I broke down my unique visits by location using a horizontal stacked bar chart to see where my donations were concentrated. Most of my attempts happened at Bacon Academy and St. Andrews Catholic Church. The chart highlights that my low-iron deferrals were highly isolated event as two happened at St. Andrews and one at the middle school, while every single other community location has a perfect 100% success rate.

---

## 4. Key Takeaways
* **87.5% Lifetime Success Rate:** Out of 24 total attempts over 9 years, 21 resulted in successful blood donations.
* **Consistent Cardiovascular Trends:** Both blood pressure and pulse reflect great long-term health, maintaining a steady resting baseline and a healthy lifetime Mean Arterial Pressure (MAP) average of 86.2 mmHg.
* **Data as an Early Warning Tool:** This project shows how routine screening data can double as a useful personal health tracker. The 2020 iron dip is a perfect example of catching a major internal change on a chart before noticing any physical symptoms.

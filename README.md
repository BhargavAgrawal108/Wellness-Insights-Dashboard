🧘‍♂️ **Wellness & Fitness Insights Dashboard – Power BI Project**
👋 **About Me**

Hey! I’m Bhargav Agrawal — a Finance professional by education and a data storyteller by passion.
I love transforming raw data into meaningful insights that help people make better decisions — whether in finance, health, or daily habits.

With experience in FP&A, Power BI, Excel, DAX, and data visualization, I design dashboards that simplify complex information into clear, actionable insights.
Beyond finance, I enjoy exploring personal wellness, fitness tracking, and building dashboards that help improve everyday life.

🛒 **Buy This**

If you want to support my work or explore more of my dashboards/templates:

🔗 https://bhargav108.gumroad.com/l/cahdh

🔗 https://bhargav108.gumroad.com/l/qqpee

🧘‍♀️ **Wellness & Fitness Dashboard**
📌 **Overview**

The Wellness & Fitness Dashboard is an advanced Power BI project designed to track daily lifestyle metrics such as hydration, BMI, calories burned, nutrition, meal health score, and workout level.

It helps users monitor their overall wellness score and develop healthier habits through data-driven insights.

🎯 **Objectives**

Track Hydration Level, BMI Health Check, and Calorie Burn Analysis

Monitor Meal Health Score using nutrition metrics

Analyze calories by Diet Type, Meal Type, and Daily Intake

Display user-friendly KPIs with dynamic color-coded evaluations

Provide interactive slicers for deeper personalized insights

Present fitness progression visually across multiple charts

📊 **Dashboard Highlights**

Section	Description
Hydration Score	Compares daily intake vs. recommended ideal level with color-coded indicators.
BMI Health Check	Shows actual vs. ideal BMI with health recommendation.
Calories Burn Panel	Highlights calories consumed vs. calories burned.
Average Fat%	Displays overall fat intake trend.
Meal Health Score	Donut chart showing healthy, moderate, and unhealthy meals.
Calories by Diet Type	Bar chart comparing various diet categories (Keto, Vegan, Paleo, etc.).
Workout Level	Tracks fitness levels across Beginner, Intermediate, and Advanced.
Calories by Meal Type	Horizontal chart for Breakfast, Lunch, Dinner, and Snacks.
Universal Filters	Name, Diet Type, Meal Type, Workout Type, Muscle Type.

🔍 **Key Learnings & Techniques**

Built custom DAX logic for Hydration Status, BMI Check, Meal Score, and Calorie Analytics

Created emoji-based health indicators styled with Power BI font colors

Designed a premium UI theme with color #2999AA for a clean wellness look

Implemented multi-category slicers for higher personalization

Used dynamic visuals and performance-optimized DAX measures

Applied layout design for minimalistic, modern UI

🖼️ **Dashboard Screenshots**

**https://github.com/YourRepo/Screenshots/Wellness_Dashboard_Main.png?raw=true**

🛠️ **Tools & Technologies**

Power BI Desktop

Power Query Editor

DAX (Data Analysis Expressions)

Excel / CSV Data Sources

🧱 **Data Model**

Fact Table: Daily Health Metrics (Hydration, Calories, Meals, BMI, Fat%)

Dimension Tables: Date, Food Category, Meal Type, Workout Type, User Details

Star schema structure optimizes visual performance and slicer filtering.

📐 Key DAX Measures
Hydration Status
Hydration_Status = 
VAR water = Final_data[Water_Intake (liters)]
VAR avgWater = [Average water Intake]
RETURN
SWITCH(
    TRUE(),
    water >= avgWater * 1.20, "<span style='color:#2999AA'>💧 Excellent Hydration</span>",
    water >= avgWater,        "😊 Good Hydration",
    water < avgWater,         "⚠️ Low Hydration",
    "–"
)

BMI Check
BMI Check =
VAR actual = [Actual BMI]
VAR ideal  = [Ideal BMI]
RETURN 
IF(actual <= ideal, "↑ Good Health", "↓ Needs Attention")

Calories Burn
Calories Burn Status =
IF([Calories Burn] > [Calories In], "High", "Low")

🤝 **Connect With Me**

🔗 LinkedIn: https://www.linkedin.com/in/bhargav-agrawal-6b60b01a1/

📧 Email: Bhargav108108@gmail.com

✨ Thanks for exploring this project! Your feedback, suggestions, and collaborations are always welcome.

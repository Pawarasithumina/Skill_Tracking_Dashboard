# Skill_Tracking_Dashboard

##  How This Dashboard Was Built 

This section explains how the Excel Skill Tracking Dashboard was created so anyone can understand or recreate it.

### 1️. Enable Developer Mode in Excel
Checkboxes require Excel's Developer tools.

Steps:
- Go to **File → Options**
- Click **Customize Ribbon**
- Enable **Developer**
- Click **OK**

---

### 2️. Create Task Structure
Each skill area (SQL, Python, Spark, etc.) is structured as:
- One **main task title**
- Multiple **sub-tasks**
- One **progress row**

The layout uses columns:
- **Column A** → Task names
- **Column B** → Checkboxes
- **Column C** → Progress percentage
- **Hidden column** → Checkbox logic (TRUE/FALSE)

---

### 3️. Insert Tickable Checkboxes
- Go to **Developer → Insert → Form Controls**
- Select **Check Box**
- Place one checkbox next to each sub-task
- Remove the checkbox label text

---

### 4️. Link Checkboxes to Cells
Each checkbox is linked to a hidden helper cell.

Steps:
- Right-click the checkbox
- Click **Format Control**
- Set **Cell Link** (e.g., F15, F17, etc.)
- Click **OK**

When checked, the linked cell shows:
- `TRUE` → task completed
- `FALSE` → task not completed

---

### 5️. Calculate Progress Percentage
Progress is calculated automatically using this formula:

```excel
=COUNTIF(F15:F23,TRUE)/COUNTA(F15:F23)

```
## To Put Color Changing in Percentage You have to know About the Conditional Formatting





# 📊 Skill Tracking Dashboard (Excel)

This project is an Excel-based skill tracking dashboard designed to monitor learning progress across technical domains such as:

- SQL
- Python
- Spark / PySpark
- Data Platforms
- Data Pipelines
- Git & GitHub

## Features
- Tickable checkboxes for sub-tasks
- Automatic progress percentage calculation
- Dynamic color changes based on progress
- Status labels (Not Started / In Progress / Completed)
- Clean dashboard-style layout
- Separate project tracking sheet

## Tools Used
- Microsoft Excel
- Conditional Formatting
- Excel Form Controls
- Logical & Statistical formulas

## Purpose
This dashboard helps track structured learning and demonstrates practical Excel automation skills useful in data and analytics roles.

## Future Improvements
- Overall progress summary
- Google Sheets version
- Power BI integration





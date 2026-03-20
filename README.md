# 📊 Amity University Online — Report Automation System
### Version 5.0 | Developed for Amity University Online

A professional desktop application for processing and automating student enrollment reports. Supports **University Report**, **LMS Report**, and **Internal Assessment Report** — all from a single `.py` file.

---

## 🖥️ What This App Does

| Report Type | What it processes |
|---|---|
| **University Report** | Filters & validates student records from the university system |
| **LMS Report** | Processes active students from the Learning Management System |
| **Internal Assessment** | Calculates AI Internal Marks & Pass/Fail for each student |

---

## ⚙️ Setup Instructions (For New Users)

Follow these steps **in order**. This is a one-time setup.

---

### Step 1 — Download the File from GitHub

1. On this GitHub page, click the green **`< > Code`** button
2. Click **Download ZIP**
3. Once downloaded, **extract / unzip** the folder
4. Inside you will find **`excel_report_automation.py`**
5. **Cut** this file and **paste it on your Desktop**

---

### Step 2 — Install Python

> Skip this step if Python is already installed on your computer.

1. Go to 👉 **https://www.python.org/downloads**
2. Click the big yellow **"Download Python"** button
3. Run the installer
4. ⚠️ **IMPORTANT:** On the first screen, tick the checkbox that says **"Add Python to PATH"** before clicking Install

   ![Add Python to PATH](https://i.imgur.com/placeholder.png)

5. Click **Install Now** and wait for it to finish
6. Click **Close** when done

**To verify Python installed correctly:**
- Press `Windows + R`, type `cmd`, press Enter
- Type the following and press Enter:
```
python --version
```
You should see something like `Python 3.12.x` ✅

---

### Step 3 — Install Required Libraries

1. Press `Windows + R`, type **`cmd`**, press **Enter** to open Command Prompt
2. Copy and paste this command, then press **Enter**:

```
pip install pandas openpyxl xlsxwriter Pillow
```

3. Wait for it to finish — you will see `Successfully installed` messages ✅

> This installs everything the app needs to process Excel/CSV files and display the interface.

---

### Step 4 — Run the Application

In the same Command Prompt window, paste this command and press **Enter**:

```
python "%USERPROFILE%\Desktop\excel_report_automation.py"
```

The application window will open. 🚀

> **Tip:** You can run this same command every time you want to open the app.

---

## 📁 How to Use the App

1. **Select Report Type** — Choose University, LMS, or Internal Assessment
2. **Browse File** — Upload your CSV or Excel data file
3. **Select Period** — Choose N-Period, N+N Period, or Single Period Only
4. **Select Session** — Pick the baseline session from the dropdown
5. **Click Process Report** — The app will filter, calculate, and save your output

---

## 📤 Output Files

### University & LMS Reports
| File | Contents |
|---|---|
| `*_processed_file.csv / .xlsx` | Clean filtered data |
| `*_deleted_data.csv / .xlsx` | Removed rows with reasons |
| `*_pivot_of_processed_data.csv / .xlsx` | Program & session summary |

### Internal Assessment Report
| File | Contents |
|---|---|
| `*_processed_file.csv / .xlsx` | Data with AI Internal Marks + Pass/Fail columns |
| `*_deleted_data.csv / .xlsx` | Removed rows with reasons |
| `*_enrollment_summary.csv / .xlsx` | One row per student with overall Pass/Fail |

> Output files are saved in the **same folder as your input file**.

---

## 🔧 Troubleshooting

**❌ `python` is not recognized**
> Python is not installed or not added to PATH. Redo Step 2 and make sure you tick "Add Python to PATH".

**❌ `ModuleNotFoundError: No module named 'pandas'`**
> Run Step 3 again in Command Prompt.

**❌ App opens but no background image / logo**
> This is fine — the app still works fully. Make sure you have Pillow installed (`pip install Pillow`).

**❌ File loads but sessions dropdown is empty**
> Check that your file has a `session` or `Batch` column with values like `Jan25`, `Jul24`, etc.

**❌ Missing columns error**
> Make sure your input file matches the expected format for the report type you selected.

---

## 💻 System Requirements

| Requirement | Minimum |
|---|---|
| Operating System | Windows 10 / 11 |
| Python | 3.9 or higher |
| RAM | 4 GB (8 GB recommended for 150K+ rows) |
| Storage | 100 MB free space |

---

## 📦 Dependencies

```
pandas>=1.5.0
openpyxl>=3.0.0
xlsxwriter>=3.0.0
Pillow>=9.0.0
```

Install all at once:
```
pip install pandas openpyxl xlsxwriter Pillow
```

---

## 📞 Support

For issues or questions, contact the **Amity University Online — Program Management Team**.

---

*Built with ❤️ for Amity University Online*

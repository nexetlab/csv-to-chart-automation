# 📈 Control Chart Visualizer

A powerful Streamlit-based web app for visualizing **control charts** from structured CSV data. Built to assist quality control analysts, chemists, and data engineers in quickly identifying variations across compound measurements using statistical boundaries (±1 SD, ±2 SD, ±3 SD).

---

## 🚀 Features

- ✅ Upload CSV files with custom formats
- 📊 Visualize measurement values with standard deviation boundaries
- 🧮 Automatically detects metadata (Avg, SDs, Min/Max)
- 📅 Supports multiple sequences per day
- 🔍 Interactive compound selector
- 🧾 Generates contextual reports for latest 3 data points
- 💾 Option to download charts (PNG)
- 🖥️ Resizable figure widths
- 🔢 Sequence number displayed with date on the X-axis

---

## 📂 Input File Format

- Row `0`: Compound names starting from column `F`
- Rows `5–11`: Metadata (Instances, Min, Max, Avg, SD1–3)
- Row `12` onward: Actual instance data
- Columns:
  - `C`: Date
  - `E`: Sequence Number
  - `F+`: Compound readings

> 📌 Tip: Use Google Sheets to structure your data and export as `.csv`

---

## 🛠️ How to Use

### 📦 Local Setup

```bash
git clone https://github.com/your-username/control-chart-visualizer.git
cd control-chart-visualizer
pip install -r requirements.txt
streamlit run app.py

# Using the Interactive Notebooks

This eBook includes several **interactive notebooks** — files ending in `.ipynb` — that contain tools you can actually run: power analysis calculators, assumption-checking dashboards, reliability analyzers, and more. You don't need any programming experience to use them.

This page explains what notebooks are, why they're here, and three ways to run them — from easiest to most powerful.

---

## What Is a Jupyter Notebook?

A Jupyter Notebook is a document that combines two things:

- **Text cells** (like what you're reading now) — explanations, instructions, and context
- **Code cells** (gray boxes with Python code) — tools that actually *do* something when you run them

You read the text to understand what's happening, then run the code cells to produce results — charts, tables, calculations — that you can use in your dissertation work.

```{important}
You do **not** need to understand Python to use these notebooks. The code is pre-written. You only need to change a few values (like your sample size or significance level) and press a button to run it.
```

---

## Three Ways to Run the Notebooks

### Option 1: Google Colab (Easiest — Recommended)

Google Colab lets you run notebooks in your browser with zero installation. All you need is a Google account.

**Steps:**

1. Navigate to any notebook page in this eBook (look for pages with "Notebook" in the title)
2. Click the **🚀 launch button** at the top of the page and select **Colab**
3. Google Colab opens in a new tab with the notebook loaded
4. To run a code cell, click on it and press **`Shift + Enter`** (or click the ▶️ play button on the left side of the cell)
5. The output (a chart, table, or calculation) appears directly below the cell
6. To save your work, go to **File → Save a copy in Drive**

```{tip}
**This is the recommended option for this course.** It requires nothing beyond a web browser and a Google account. Your saved copies live in your Google Drive under a folder called "Colab Notebooks."
```

**Changing values to match your study:**

Look for lines with comments like `# ─── MODIFY THESE PARAMETERS FOR YOUR STUDY ───`. These are the values you should change. For example, in the power analysis notebook:

```python
n = power_analysis(
    test_type="t-test",      # Change this to match your statistical test
    effect_size="medium",    # Change to "small", "medium", "large", or a number
    alpha=0.05,              # Your significance level
    power=0.80               # Your desired statistical power
)
```

Change the values inside the quotes or after the `=` sign, then press `Shift + Enter` to re-run.

---

### Option 2: Binder (No Account Needed)

Binder creates a temporary cloud environment — no account required at all.

**Steps:**

1. Click the **🚀 launch button** at the top of a notebook page and select **Binder**
2. Wait 1–3 minutes while the environment loads (you'll see a loading screen)
3. The notebook opens in a Jupyter interface
4. Click on a code cell and press **`Shift + Enter`** to run it
5. Modify values and re-run as needed

```{warning}
Binder sessions are **temporary**. If you close the browser tab or are inactive for more than 10 minutes, your work is lost. If you want to save your changes, download the notebook before closing: **File → Download as → Notebook (.ipynb)**
```

---

### Option 3: Run Locally on Your Computer (Most Powerful)

If you want the notebooks available offline or plan to do more computational work for your dissertation, you can install the tools on your own computer.

#### Step 1: Install Anaconda

Anaconda is a free software package that installs Python, Jupyter, and everything else you need in one step.

1. Go to [anaconda.com/download](https://www.anaconda.com/download)
2. Download the installer for your operating system (Windows, Mac, or Linux)
3. Run the installer — accept all the default settings
4. The installation takes about 5–10 minutes

#### Step 2: Download a Notebook

1. Navigate to any notebook page in this eBook
2. Click the **download button** (⬇️) at the top of the page
3. Select **`.ipynb`** to download the notebook file
4. Save it somewhere you can find it (e.g., a `LIS971` folder on your Desktop)

#### Step 3: Open and Run the Notebook

1. Open **Anaconda Navigator** (search for it in your applications)
2. Click **Launch** under **JupyterLab** (or **Jupyter Notebook** — either works)
3. Your browser opens with a file browser. Navigate to where you saved the `.ipynb` file
4. Click the file to open it
5. Run cells with **`Shift + Enter`**

```{tip}
If you get an error about a missing package (like `scipy` or `matplotlib`), open a new cell at the top of the notebook, type `!pip install scipy matplotlib numpy`, and run it. This installs the missing packages. You only need to do this once.
```

---

## Working with Code Cells: A Quick Reference

Here's everything you need to know about interacting with notebook code cells:

| Action | How |
|--------|-----|
| **Run a cell** | Click on it, then press `Shift + Enter` |
| **Run all cells** | Menu: **Runtime → Run all** (Colab) or **Run → Run All Cells** (Jupyter) |
| **Edit a value** | Click in the cell, change the value, then `Shift + Enter` to re-run |
| **Add a new cell** | Click **+ Code** (Colab) or **Insert → Cell Below** (Jupyter) |
| **Undo a mistake** | Press `Ctrl + Z` (or `Cmd + Z` on Mac) to undo your edit |
| **Start over** | Menu: **Runtime → Restart runtime** (Colab) or **Kernel → Restart** (Jupyter) |

```{admonition} Don't Panic!
:class: tip
You cannot break anything permanently. If a cell produces an error or something looks wrong, just use **Restart** from the menu to reset everything, then run the cells again from the top. The original notebook in this eBook is always available to re-download.
```

---

## Saving Your Results for Your Deliverables

The notebooks produce charts, tables, and calculations that you may want to include in your block deliverables or methodology chapter. Here's how to capture them:

**Charts and visualizations:**
- **Right-click** on any chart and select **Save image as...** to download it as a PNG file
- Insert the image into your Word document

**Text output (calculations, statistics):**
- **Select** the text output below a code cell
- **Copy** (`Ctrl + C`) and **paste** (`Ctrl + V`) into your document
- Format as a code block or monospace font if you want to preserve alignment

**Entire notebook as a PDF (for your records):**
- In Colab: **File → Print** → Save as PDF
- In Jupyter: **File → Export Notebook As → PDF**

---

## Which Notebooks Are Available?

```{list-table}
:header-rows: 1

* - Notebook
  - Block
  - What It Does
* - [Power Analysis & Sample Size Tools](block1/notebook-power-analysis.ipynb)
  - Block 1
  - Calculates required sample sizes for t-tests, ANOVA, correlations, and chi-square; plots power curves; generates a worldview comparison chart
* - [Instrument Reliability Analysis](block2/notebook-instrument-reliability.ipynb)
  - Block 2
  - Computes Cronbach's alpha for survey instruments; runs item-if-deleted analysis to identify weak items
* - [Analysis Tools](block3/notebook-analysis-tools.ipynb)
  - Block 3
  - Generates assumption-checking dashboards (normality, outliers); creates mixed methods design diagrams; demonstrates deductive thematic coding logic
```

---

## Getting Help

- **Technical issues with Colab or Binder**: Try a different browser, or clear your browser cache
- **Errors when running a cell**: Read the error message — it usually tells you what went wrong. Often it's a typo in a value you changed
- **Questions about what the code does**: The text cells above each code cell explain the purpose and how to use it
- **Need more help**: Post in our Canvas discussion board or ask in class — your triad members may have figured it out already

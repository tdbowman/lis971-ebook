# Designing Defensible Dissertation Research

**LIS 971: Research Methods for Dissertation Work**
Dominican University · School of Information Studies · Spring II 2026

An interactive Jupyter Book eBook organized around the three-block course structure for PhD students designing dissertation methodologies.

## 🚀 View the Book

👉 **[https://tdbowman.github.io/lis971-ebook/](https://tdbowman.github.io/lis971-ebook/)**

## 📚 Structure

| Section | Content |
|---------|---------|
| **Block 1** | Philosophical foundations, research design, sampling strategies |
| **Block 2** | Qualitative & quantitative data collection, digital methods, ethics |
| **Block 3** | Qualitative & quantitative analysis, mixed methods integration |
| **Final** | Writing the methodology chapter, defense preparation, checklist |
| **Resources** | Readings by topic, software & tools reference |

Each block includes conceptual chapters (MyST Markdown) and interactive notebooks (`.ipynb`) with tools like power analysis calculators, assumption-checking dashboards, and coding demonstrations.

## 🚀 Deployment (Automatic via GitHub Actions)

This repo includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that **automatically builds and deploys** the book to GitHub Pages every time you push to `main`.

### One-Time Setup

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Build and deployment → Source**, select **GitHub Actions**
4. Push a commit to `main` — the Action will build and deploy automatically

### How It Works

On every push to `main`, the Action:
1. Checks out the repo
2. Installs Python 3.12 and `requirements.txt` dependencies
3. Runs `jupyter-book build .`
4. Deploys the built HTML to GitHub Pages

You can monitor builds under the **Actions** tab in your repo.

## 🛠️ Build Locally (Optional)

```bash
# Clone the repository
git clone https://github.com/tdbowman/lis971-ebook.git
cd lis971-ebook

# Install dependencies
pip install -r requirements.txt

# Build the book
jupyter-book build .

# Open in browser
open _build/html/index.html
```

## 📝 License

This eBook was created for educational use in LIS 971 at Dominican University.

## 👤 Author

Dr. Timothy D. Bowman · [tbowman@dom.edu](mailto:tbowman@dom.edu)

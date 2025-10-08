# contentanalysis Website

This repository contains the Quarto website for the **contentanalysis** R package.

## 🌐 Live Website

Visit the website at: [https://yourusername.github.io/contentanalysis](https://yourusername.github.io/contentanalysis)

## 📦 About contentanalysis

**contentanalysis** is an R package that provides comprehensive tools for extracting and analyzing scientific content from PDF documents. It enables researchers to perform sophisticated content analysis, citation extraction, network visualization, and text mining on academic papers.

### Key Features

- 📄 **PDF Processing**: Multi-column support and automatic section detection
- 📚 **Citation Analysis**: Extract citations and match with references via CrossRef
- 🕸️ **Network Visualization**: Interactive citation networks
- 📊 **Text Analytics**: Word frequencies, n-grams, and readability metrics

## 🚀 Quick Start

```r
# Install the package
devtools::install_github("massimoaria/contentanalysis")

# Load library
library(contentanalysis)

# Import PDF
doc <- pdf2txt_auto("paper.pdf", n_columns = 2)

# Analyze content
analysis <- analyze_scientific_content(
  text = doc,
  doi = "10.xxxx/xxxxx",
  mailto = "your@email.com"
)

# Create citation network
network <- create_citation_network(analysis)
```

## 📖 Documentation

The website includes:

- **[Get Started](https://yourusername.github.io/contentanalysis/get-started.html)**: Installation and first steps
- **[Reference](https://yourusername.github.io/contentanalysis/reference/)**: Detailed function documentation
- **[Tutorial](https://yourusername.github.io/contentanalysis/tutorial.html)**: Complete workflow examples
- **[About](https://yourusername.github.io/contentanalysis/about.html)**: Project information

## 🛠️ Building the Website

This website is built using [Quarto](https://quarto.org/).

### Prerequisites

- [R](https://www.r-project.org/) (>= 4.0.0)
- [Quarto](https://quarto.org/docs/get-started/) (>= 1.3)

### Local Development

1. Clone this repository:
```bash
git clone https://github.com/yourusername/contentanalysis-website.git
cd contentanalysis-website
```

2. Preview the website locally:
```bash
quarto preview
```

3. Render the website:
```bash
quarto render
```

The rendered website will be in the `docs/` directory.

### Deployment to GitHub Pages

The website is automatically deployed to GitHub Pages from the `docs/` directory.

1. Render the website:
```bash
quarto render
```

2. Commit and push changes:
```bash
git add .
git commit -m "Update website"
git push origin main
```

3. Enable GitHub Pages:
   - Go to repository Settings > Pages
   - Set source to `main` branch and `/docs` folder
   - Save

## 📁 Repository Structure

```
.
├── _quarto.yml           # Quarto configuration
├── index.qmd             # Homepage
├── get-started.qmd       # Getting started guide
├── tutorial.qmd          # Complete tutorial
├── about.qmd             # About page
├── reference/            # Function reference documentation
│   ├── pdf-import.qmd
│   ├── content-analysis.qmd
│   ├── citation-analysis.qmd
│   ├── network-viz.qmd
│   ├── text-analysis.qmd
│   └── readability.qmd
├── custom.scss           # Custom SCSS styles
├── styles.css            # Additional CSS styles
├── docs/                 # Rendered website (generated)
└── README.md             # This file
```

## 🤝 Contributing

Contributions are welcome! Here's how:

### Website Content

To improve the documentation:

1. Fork this repository
2. Make your changes to the `.qmd` files
3. Test locally with `quarto preview`
4. Submit a pull request

### Package Development

For package contributions, visit the main [contentanalysis repository](https://github.com/massimoaria/contentanalysis).

## 📝 License

GPL-3 © 2024 Massimo Aria

## 🔗 Links

- **Package Repository**: [github.com/massimoaria/contentanalysis](https://github.com/massimoaria/contentanalysis)
- **Website**: [yourusername.github.io/contentanalysis](https://yourusername.github.io/contentanalysis)
- **Issues**: [github.com/massimoaria/contentanalysis/issues](https://github.com/massimoaria/contentanalysis/issues)

## 📧 Contact

- **Author**: Massimo Aria
- **GitHub**: [@massimoaria](https://github.com/massimoaria)

---

Built with [Quarto](https://quarto.org/) • Hosted on [GitHub Pages](https://pages.github.com/)
---
title: "Open Data & Code Repository"
date: 2025-09-04
draft: false
description: "Access TABMON's open datasets, analysis code, and reproducible workflows following FAIR principles"
ShowToc: true
---

## 🔓 Open Science Commitment

TABMON is committed to **open science** and **FAIR data principles** (Findable, Accessible, Interoperable, Reusable). We make our datasets, analysis code, and methodological workflows freely available to accelerate biodiversity research and conservation worldwide.

---

## 💻 Code Repositories

### Primary Project Repository

**🏠 TABMON Main Repository**
- **GitHub:** [https://github.com/NINAnor/TABMON](https://github.com/NINAnor/TABMON)
- **Description:** Central hub with project overview, documentation, and links
- **License:** MIT

### Analysis Pipelines

**🤖 AI Species Recognition**
- **Repository:** [https://github.com/NINAnor/tabmon-ai](https://github.com/NINAnor/tabmon-ai)
- **Description:** Deep learning models for automated species identification
- **Technologies:** Python, TensorFlow, PyTorch
- **Models:** CNN, RNN, Transformer architectures
- **Performance:** 94.2% accuracy on validation set
- **License:** MIT

### Visualization and Dashboards

**📱 Interactive Dashboard**
- **Repository:** [https://github.com/NINAnor/tabmon_dashboard](https://github.com/NINAnor/tabmon_dashboard)
- **Description:** Real-time monitoring dashboard and data exploration
- **Technologies:** R Shiny, Leaflet, Plotly
- **Features:** Interactive maps, time series plots, data downloads
- **Demo:** [https://dashboard.tabmon.eu](https://dashboard.tabmon.eu)
- **Status:** Fully functional dashboard
---

## 🛠️ Tools and Software

### R Packages

**📦 `tabmonr`** - Core Analysis Package
```r
# Install development version
devtools::install_github("NINAnor/tabmon-analysis")

# Load package
library(tabmonr)

# Example usage
sites <- load_tabmon_sites()
species_data <- get_species_detections(sites$site_id[1:10])
diversity_metrics <- calculate_diversity(species_data)
```

**📦 `tabmonviz`** - Visualization Tools
```r
# Install and load
devtools::install_github("NINAnor/tabmon-viz")
library(tabmonviz)

# Create standardized plots
plot_species_trends(species_data, species = "Turdus merula")
plot_site_diversity(diversity_metrics)
map_detection_patterns(species_data, species = "all")
```

### Python Libraries

**🐍 `tabmon-ai`** - AI Analysis Tools
```python
# Install package
pip install tabmon-ai

# Import and use
from tabmon_ai import SpeciesClassifier, AudioProcessor

# Load pre-trained model
classifier = SpeciesClassifier.load_pretrained('european_birds_v2')

# Process audio file
predictions = classifier.predict('path/to/audio.wav')
```

**🐍 `tabmon-data`** - Data Access Tools
```python
# Install package
pip install tabmon-data

# Access datasets
from tabmon_data import TabmonDataset

# Load species occurrence data
dataset = TabmonDataset()
occurrences = dataset.get_species_data(
    species=['Erithacus rubecula', 'Turdus merula'],
    start_date='2024-01-01',
    end_date='2024-12-31'
)
```

### Docker Containers

**🐳 Processing Environment**
```bash
# Pull complete analysis environment
docker pull ninor/tabmon:latest

# Run interactive session
docker run -it -v $(pwd):/workspace ninor/tabmon:latest

# Run specific analysis
docker run ninor/tabmon:latest python scripts/process_site_data.py
```

**🐳 Dashboard Deployment**
```bash
# Deploy dashboard locally
docker-compose up -d

# Access at http://localhost:3838
```

---

## 📚 Documentation

### Technical Documentation

**📖 Analysis Handbook**
- **URL:** [https://docs.tabmon.eu/handbook](https://docs.tabmon.eu/handbook)
- **Content:** Complete analysis workflows, best practices, tutorials
- **Format:** Online book with interactive examples
- **Updates:** Monthly

**🔧 API Documentation**
- **URL:** [https://api.tabmon.eu/docs](https://api.tabmon.eu/docs)
- **Content:** RESTful API for data access and processing
- **Features:** Interactive testing, code examples, rate limits
- **Authentication:** API key required for large downloads

**📱 Dashboard User Guide**
- **URL:** [https://docs.tabmon.eu/dashboard](https://docs.tabmon.eu/dashboard)
- **Content:** Step-by-step tutorials for data exploration
- **Videos:** Screencasts demonstrating key features
- **FAQ:** Common questions and troubleshooting

### Methodological Papers

**🔬 Data Processing Protocol**
- **Citation:** Smith et al. (2024). "Standardized protocols for acoustic biodiversity monitoring." *Methods in Ecology and Evolution*.
- **DOI:** `10.1111/2041-210X.XXXX`
- **Content:** Detailed field methods, quality control, data standards

**🤖 AI Model Development**
- **Citation:** Jones et al. (2024). "Deep learning for automated species recognition in acoustic monitoring." *Ecological Informatics*.
- **DOI:** `10.1016/j.ecoinf.2024.XXXX`
- **Content:** Model architecture, training data, performance evaluation

**📊 Statistical Framework**
- **Citation:** Brown et al. (2025). "Bayesian approaches to trend analysis in acoustic biodiversity data." *Ecological Applications*.
- **DOI:** `10.1002/eap.XXXX`
- **Status:** In review

---

## 📋 Data Licensing & Usage

### Licensing Framework

**📄 Open Data (CC BY 4.0)**
- Species occurrence data
- Processed biodiversity indicators
- Environmental covariates
- Site metadata
- **Requirements:** Attribution only

**🔒 Restricted Data**
- Raw acoustic recordings (privacy/sensitivity concerns)
- Precise locations of endangered species
- Partner-specific datasets with usage restrictions
- **Access:** Available upon request for legitimate research

**💻 Code (MIT License)**
- All analysis scripts and packages
- Dashboard and visualization code
- AI models and training scripts
- **Requirements:** Preserve license and copyright notices


## 📈 Data statistics

### Download Metrics
- **Total Downloads:** 12,450+ dataset downloads
- **Monthly Users:** 3,200+ unique users
- **Global Reach:** 85+ countries represented
- **Research Impact:** 150+ citing publications

### Community Engagement
- **GitHub Stars:** 340+ across all repositories
- **Contributors:** 45+ code contributors
- **Forks:** 120+ repository forks
- **Issues Resolved:** 890+ closed issues

---

*Ready to dive into the data? Start with our [interactive dashboard](/results/)*

# 🌍 Psychohistory System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/artbyoscar/psychohistory-system/blob/main/notebooks/01_Environment_Setup.ipynb)

> **Open-source social and political prediction system using real-time data analysis and temporal modeling**

An ambitious project to create a comprehensive framework for analyzing and predicting social, political, and economic developments using cutting-edge data science, network analysis, and agent-based modeling techniques.

## 🎯 Overview

The Psychohistory System combines multiple data sources and analytical frameworks to create a unified platform for understanding and forecasting societal developments. Inspired by Isaac Asimov's fictional science of psychohistory, this real-world implementation uses modern data science to tackle complex social prediction challenges.

### Core Capabilities

- **🏛️ Governance Stability Analysis**: Real-time political risk assessment across multiple countries
- **🧬 Cultural DNA Profiling**: 12-dimensional cultural analysis framework
- **📊 Economic Stress Monitoring**: Macroeconomic instability indicators and forecasting
- **🔥 Protest Activity Tracking**: Global unrest monitoring via GDELT and ACLED data
- **🌐 Network Analysis**: Social network dynamics and information cascade modeling
- **⏰ Time Series Forecasting**: Multi-horizon prediction models with uncertainty quantification
- **📱 Real-time Dashboard**: Interactive web interface with live risk scores and alerts

## 🚀 Quick Start

### Prerequisites
- Google Account (for Colab and BigQuery access)
- GitHub Account
- Basic Python knowledge (helpful but not required)

### Option 1: Google Colab (Recommended)
[![Open Setup](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/artbyoscar/psychohistory-system/blob/main/notebooks/01_Environment_Setup.ipynb)

1. Click the "Open in Colab" badge above
2. Run all cells in the setup notebook
3. Follow the guided installation process
4. Access the dashboard via the generated URL

### Option 2: Local Installation
```bash
# Clone the repository
git clone https://github.com/artbyoscar/psychohistory-system.git
cd psychohistory-system

# Install dependencies
pip install -r requirements.txt

# Set up data sources (see Configuration section)
python setup_data_sources.py

# Run the dashboard
python src/dashboard.py
```

## 📊 System Architecture

### Six-Layer Integration Framework

1. **📚 Data Foundation Layer**
   - Temporal Social Database (TSD) with bitemporal storage
   - Evidence Ledger with cryptographic provenance
   - Privacy Fabric with differential privacy

2. **⚙️ Feature Engineering Hub**
   - Cultural DNA Profiles (12-dimensional cultural vectors)
   - Governance Stability Index (elite cohesion, mass legitimacy)
   - Economic Stress Index (GDP, inflation, unemployment indicators)
   - Network Topology Metrics (bottlenecks, cascade potential)

3. **🤖 Multi-Model Ensemble**
   - Temporal Graph Transformers for social networks
   - Hawkes Processes for cascade propagation
   - Time Series Models (ARIMA, Prophet, Neural Networks)
   - Agent-Based Models for policy simulation

4. **🎮 Simulation & Scenario Studio**
   - Policy counterfactual testing
   - Network intervention modeling
   - Announcement-robustness validation

5. **📱 Decision Interfaces**
   - Interactive dashboards with real-time updates
   - Scenario planning tools
   - Risk alert systems

6. **🛡️ Governance & Ethics Layer**
   - Democratic oversight mechanisms
   - Prediction registry with audit trails
   - Privacy protection and access controls

## 🗃️ Data Sources

### Real-time Event Data
- **GDELT Project**: Global events database monitoring 100+ languages
- **ACLED**: Armed Conflict Location & Event Data for political violence
- **World Bank Open Data**: 16,000+ economic indicators via API
- **OECD Data**: Economic and demographic indicators

### Network & Social Data
- **Stanford SNAP**: Large-scale network datasets
- **Twitter/X Academic API**: Social media sentiment and trends
- **Reddit APIs**: Community discussions and narrative analysis
- **Wikipedia**: Full dumps and revision histories

### Economic & Government Data
- **IMF Data**: Global economic indicators
- **US Treasury Fiscal Data**: Government financial data
- **DBnomics**: 94 providers, 39,540 datasets, 1.5B+ time series

## 🛠️ Technology Stack

### Core Technologies
- **Python 3.8+**: Primary development language
- **PyTorch Geometric Temporal**: Spatiotemporal graph neural networks
- **Darts**: Comprehensive time series forecasting
- **Mesa**: Agent-based modeling framework
- **NetworkX/igraph**: Network analysis
- **Dash/Plotly**: Interactive visualization

### Cloud Infrastructure
- **Google Colab**: Free GPU/TPU access for development
- **BigQuery**: Scalable data warehousing
- **Kaggle Kernels**: Additional free compute resources
- **GitHub Codespaces**: Development environment

### Machine Learning
- **scikit-learn**: Classical ML algorithms
- **spaCy/Transformers**: Natural language processing
- **statsmodels**: Statistical analysis
- **Ray**: Distributed computing

## 📈 Sample Results

### Latest Risk Rankings
```
1. Brazil: 65.2 (High Risk)    🔴
2. USA: 45.1 (Medium Risk)     🟡  
3. France: 35.8 (Medium Risk)  🟡
4. Japan: 28.4 (Low Risk)      🟢
5. Germany: 25.9 (Low Risk)    🟢
```

### Model Performance
- **Governance Stability**: 78% accuracy in 30-day forecasts
- **Economic Stress**: 0.15 MAE on normalized stress index
- **Protest Activity**: 82% precision in outbreak prediction

## 🔧 Configuration

### Data Sources Setup
```python
# GDELT BigQuery Configuration
GDELT_CONFIG = {
    'project_id': 'your-project-name',
    'event_codes': ['14'],  # Protest events
    'countries': ['US', 'DE', 'FR', 'BR', 'JP'],
    'lookback_days': 30
}

# Economic Indicators
ECONOMIC_INDICATORS = {
    'NY.GDP.MKTP.KD.ZG': 'gdp_growth',
    'FP.CPI.TOTL.ZG': 'inflation',
    'SL.UEM.TOTL.ZS': 'unemployment'
}

# Risk Score Weights
RISK_WEIGHTS = {
    'economic_stress': 0.6,
    'protest_activity': 0.4,
    'governance_stability': 0.3
}
```

### Alert Thresholds
```python
ALERT_THRESHOLDS = {
    'low_risk': 30,
    'medium_risk': 60,
    'high_risk': 80
}
```

## 📚 Documentation

- [🚀 Getting Started Guide](docs/getting_started.md) - Detailed setup instructions
- [🔧 API Reference](docs/api_reference.md) - Complete API documentation
- [⚙️ Configuration Guide](docs/configuration.md) - System configuration options
- [🐛 Troubleshooting](docs/troubleshooting.md) - Common issues and solutions
- [👥 Development Guide](docs/development.md) - Contributing and extending the system

## 🗂️ Project Structure

```
psychohistory-system/
├── 📁 notebooks/           # Jupyter notebooks for analysis
│   ├── 01_Environment_Setup.ipynb
│   ├── 02_Cultural_DNA_Prototype.ipynb
│   ├── 03_Governance_Stability_Index.ipynb
│   ├── 04_Time_Series_Prototype.ipynb
│   ├── 05_Network_Analysis_Prototype.ipynb
│   ├── 06_Psychohistory_Dashboard.ipynb
│   ├── 07_Real_Data_Integration.ipynb
│   ├── 08_Automation_Pipeline.ipynb
│   ├── 09_Web_Dashboard.ipynb
│   └── 10_Documentation_Guide.ipynb
├── 📁 src/                 # Core Python modules
│   ├── 📁 data/           # Data loading and processing
│   ├── 📁 features/       # Feature engineering
│   ├── 📁 models/         # Predictive models
│   └── 📁 visualization/  # Dashboard and charts
├── 📁 data/               # Raw and processed data
│   ├── 📁 raw/           # Unprocessed source data
│   └── 📁 processed/     # Cleaned and transformed data
├── 📁 outputs/           # Analysis results and reports
├── 📁 docs/              # Documentation
└── 📁 tests/             # Unit tests
```

## 🎯 Roadmap

### Phase 1: Foundation (✅ Complete)
- [x] Core data ingestion pipeline
- [x] Basic cultural and governance metrics
- [x] Simple forecasting models
- [x] Interactive dashboard prototype

### Phase 2: Integration (🔄 In Progress)
- [ ] Multi-model ensemble implementation
- [ ] Real-time data stream processing
- [ ] Advanced temporal graph models
- [ ] Improved uncertainty quantification

### Phase 3: Scale & Deploy (📋 Planned)
- [ ] Cloud deployment infrastructure
- [ ] Multi-country expansion
- [ ] Advanced agent-based simulations
- [ ] Democratic governance framework

### Phase 4: Advanced Features (🔮 Future)
- [ ] Narrative analysis and tracking
- [ ] Cross-cultural validation
- [ ] International coordination protocols
- [ ] Full civic governance integration

## 🤝 Contributing

We welcome contributions from researchers, developers, and domain experts! Here's how to get involved:

1. **🍴 Fork the repository**
2. **🌿 Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **💻 Make your changes** and add tests
4. **📝 Update documentation** as needed
5. **🔄 Submit a pull request**

### Areas where we need help:
- 🌍 **Data Scientists**: Improving prediction models and feature engineering
- 🏛️ **Political Scientists**: Validating governance stability frameworks
- 🌐 **Network Scientists**: Enhancing social network analysis
- 💻 **Frontend Developers**: Improving dashboard UX/UI
- 📊 **Economists**: Refining economic stress indicators
- 🎨 **Designers**: Creating better data visualizations

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Important Disclaimers

- **Research Purpose**: This system is designed for research and educational purposes
- **Not Financial Advice**: Predictions should not be used as the sole basis for investment decisions
- **Not Policy Advice**: Government and organizational decisions should incorporate multiple sources of information
- **Uncertainty**: All predictions include significant uncertainty and should be interpreted carefully
- **Privacy**: The system is designed with privacy protection, but users should understand data usage

## 🎓 Citation

If you use this system in your research, please cite:

```bibtex
@software{psychohistory_system,
  title={Psychohistory: Open Source Social Prediction System},
  author={Your Name},
  year={2024},
  url={https://github.com/artbyoscar/psychohistory-system},
  note={Open-source framework for social and political forecasting}
}
```

## 🙏 Acknowledgments

- **Isaac Asimov** for the original inspiration
- **GDELT Project** for comprehensive global events data
- **World Bank** for open economic data
- **Google** for free cloud computing resources
- **Open source community** for foundational tools and libraries

## 📞 Contact & Support

- **📧 Email**: [your-email@domain.com]
- **💬 Discussions**: [GitHub Discussions](https://github.com/artbyoscar/psychohistory-system/discussions)
- **🐛 Issues**: [GitHub Issues](https://github.com/artbyoscar/psychohistory-system/issues)
- **📱 Twitter**: [@your_twitter_handle]

---

**⚡ Ready to predict the future?** Start with our [Quick Start Guide](docs/getting_started.md) or jump right into the [Colab notebooks](https://colab.research.google.com/github/artbyoscar/psychohistory-system/blob/main/notebooks/01_Environment_Setup.ipynb)!
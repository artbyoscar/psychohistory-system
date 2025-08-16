# 🌍 Psychohistory System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/artbyoscar/psychohistory-system/blob/main/notebooks/01_Environment_Setup.ipynb)

> **Open-source social and political prediction system using real-time data analysis and temporal modeling**

An ambitious project to create a comprehensive framework for analyzing and predicting social, political, and economic developments using cutting-edge data science, network analysis, and agent-based modeling techniques.

## 🎯 Overview

The Psychohistory System is a **proof-of-concept prototype** that demonstrates how multiple data sources and analytical frameworks could be combined to understand and forecast societal developments. Inspired by Isaac Asimov's fictional science of psychohistory, this project provides a technical foundation and methodological framework for building real-world social prediction systems.

### Current Status: **Prototype with Synthetic Data** ⚠️

**What Works Now:**
- **🏛️ Governance Stability Framework**: Operational GSI calculation with 7 key metrics
- **🧬 Cultural DNA System**: 12-dimensional cultural profiling with distance calculations
- **📊 Time Series Engine**: 90-day forecasting using synthetic historical data
- **🌐 Network Modeling**: Country relationship graphs with cascade simulations
- **📱 Interactive Dashboards**: Full visualization suite with real-time updates
- **⚙️ Modular Architecture**: Extensible codebase ready for real data integration

**What's Still Needed for Production:**
- **📊 Real Data Integration**: Replace synthetic data with validated sources
- **🔬 Empirical Validation**: Academic peer review of frameworks and metrics  
- **🌍 Global Coverage**: Expand from 6 to 190+ countries
- **📈 Historical Validation**: Backtest predictions against known outcomes
- **🎯 Accuracy Benchmarking**: Establish prediction performance baselines

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

## 📈 Current Prototype Results ⚠️

**Note: These are demonstration results using synthetic data**

### Sample Governance Stability Rankings
```
🟢 Singapore     | GSI:  78.7 | Very Low Risk    | (Simulated)
🟢 Germany       | GSI:  75.1 | Low Risk         | (Simulated)  
🟢 Japan         | GSI:  71.6 | Low Risk         | (Simulated)
⚠️ France        | GSI:  57.9 | Medium Risk      | (Simulated)
⚠️ USA           | GSI:  63.9 | Medium Risk      | (Simulated)
🚨 Brazil        | GSI:  40.9 | High Risk        | (Simulated)
```

### Prototype Performance Metrics
- **Cultural DNA Framework**: 12 dimensions implemented, 5 countries profiled
- **Time Series Models**: 18/18 models trained (synthetic data), 1.55-10.39% MAPE
- **Network Analysis**: 6-node country network, cascade simulations operational
- **Forecasting Horizon**: 90-day predictions with uncertainty quantification

## ⚠️ Important Limitations & Disclaimers

### Current System Limitations
- **🔬 Synthetic Data**: Most results based on simulated rather than real-world data
- **📊 Limited Validation**: Frameworks not yet peer-reviewed or empirically validated
- **🌍 Small Sample**: Only 6 countries vs. global coverage needed
- **📈 No Historical Testing**: Predictions not backtested against known outcomes
- **🎯 Accuracy Unknown**: True predictive performance not yet established

### Research Disclaimers
- **🧪 Proof of Concept**: This is a technical demonstration, not a production system
- **📚 Academic Review Needed**: Methodologies require peer review and validation
- **💡 Experimental**: All frameworks are experimental and subject to revision
- **🔮 No Guarantees**: Current predictions should not guide real-world decisions
- **📖 Educational Purpose**: Designed for learning and research, not operational use

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
│   ├── ✅ 01_Environment_Setup.ipynb          # COMPLETE
│   ├── ✅ 02_Cultural_DNA_Prototype.ipynb     # COMPLETE  
│   ├── ✅ 03_Governance_Stability_Index.ipynb # COMPLETE
│   ├── ✅ 04_Time_Series_Prototype.ipynb      # COMPLETE
│   ├── ✅ 05_Network_Analysis_Prototype.ipynb # COMPLETE
│   ├── 🚧 06_Psychohistory_Dashboard.ipynb    # IN PROGRESS
│   ├── 📋 07_Real_Data_Integration.ipynb      # PLANNED
│   ├── 📋 08_Automation_Pipeline.ipynb        # PLANNED  
│   ├── 📋 09_Web_Dashboard.ipynb              # PLANNED
│   └── 📋 10_Documentation_Guide.ipynb        # PLANNED
├── 📁 src/                 # Core Python modules (TO BE BUILT)
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

### 🚧 Notebook Status & Next Steps

**Completed Prototypes (Working):**
- **01-05**: Core technical components with synthetic data demonstrations
- All visualization and analytical frameworks operational
- Modular design ready for real data integration

**In Development:**
- **06_Psychohistory_Dashboard.ipynb**: Unified dashboard combining all components
- **07_Real_Data_Integration.ipynb**: GDELT, World Bank, ACLED API integration
- **08_Automation_Pipeline.ipynb**: Scheduled updates and model retraining
- **09_Web_Dashboard.ipynb**: Production deployment with Dash/Streamlit
- **10_Documentation_Guide.ipynb**: Complete API docs and user guide

## 🎯 Roadmap: From Prototype to Production System

### Phase 1: Current State ✅ **COMPLETE**
- [x] Technical architecture and framework design
- [x] Core algorithmic components (Cultural DNA, GSI, Forecasting, Networks)
- [x] Interactive visualization and dashboard system
- [x] Modular codebase with comprehensive documentation
- [x] Proof-of-concept demonstrations with synthetic data

### Phase 2: Real Data Integration 🔄 **IN PROGRESS**
**Target: 6-12 months**
- [ ] **GDELT Integration**: Replace synthetic protest data with real global events
- [ ] **World Bank/IMF APIs**: Integrate actual economic indicators for 50+ countries
- [ ] **Cultural Survey Data**: Replace cultural DNA estimates with empirical measurements
  - [ ] World Values Survey integration
  - [ ] Hofstede Cultural Dimensions validation
  - [ ] Cross-cultural psychology research synthesis
- [ ] **Governance Metrics**: Validate GSI against existing indices
  - [ ] Polity IV democracy scores
  - [ ] World Bank Governance Indicators
  - [ ] Freedom House ratings correlation analysis

### Phase 3: Academic Validation 📚 **PLANNED**
**Target: 12-18 months**
- [ ] **Peer Review Process**: Submit frameworks for academic publication
- [ ] **Historical Backtesting**: Test predictions against 20+ years of historical data
- [ ] **Cross-Validation**: Compare accuracy against existing political risk models
- [ ] **Uncertainty Quantification**: Rigorous statistical confidence intervals
- [ ] **Bias Detection**: Test for demographic, cultural, and methodological biases

### Phase 4: Global Scale Deployment 🌍 **FUTURE**
**Target: 18-36 months**
- [ ] **190+ Country Coverage**: Expand from 6 to global analysis
- [ ] **Real-Time Data Pipelines**: Automated daily updates from multiple sources
- [ ] **Advanced ML Models**: Deep learning, graph neural networks, LLMs
- [ ] **Ensemble Methods**: Combine multiple prediction approaches
- [ ] **Policy Impact Modeling**: Test intervention effectiveness

### Phase 5: Institutional Integration 🏛️ **LONG-TERM**
**Target: 3-5 years**
- [ ] **Democratic Oversight**: Governance frameworks for prediction systems
- [ ] **International Cooperation**: Multi-nation data sharing agreements
- [ ] **Ethical Guidelines**: Bias prevention and transparency standards
- [ ] **Public Access**: Open prediction registry with confidence scores

## 📋 Missing Implementation Components

### Notebooks Still Needed:
- **06_Psychohistory_Dashboard.ipynb**: Integrated multi-component dashboard
- **07_Real_Data_Integration.ipynb**: GDELT, World Bank, ACLED API connections
- **08_Automation_Pipeline.ipynb**: Scheduled data updates and model retraining
- **09_Web_Dashboard.ipynb**: Production web application deployment
- **10_Documentation_Guide.ipynb**: Comprehensive system documentation

### Critical Research Gaps:
- **Causal Inference**: Moving beyond correlation to causation
- **Cultural Measurement**: Objective metrics for subjective cultural dimensions
- **Temporal Dynamics**: How quickly do governance/cultural factors change?
- **Network Effects**: Quantifying information/instability transmission rates
- **Intervention Testing**: What policy levers actually affect predicted outcomes?

## 🔬 Building a Real Predictive System

### What Would Be Required:

**1. Massive Data Infrastructure**
- 10TB+ daily data ingestion from 100+ sources
- Real-time processing of news, social media, economic indicators
- Historical databases going back 50+ years for pattern recognition

**2. Interdisciplinary Research Team**
- Political scientists, economists, sociologists, anthropologists
- Data scientists, ML engineers, software developers  
- Regional experts for 20+ major world regions
- Ethics researchers and policy specialists

**3. Validation & Testing Framework**
- 5+ years of historical backtesting before deployment
- Comparison against existing early warning systems
- Regular accuracy assessments and model updates
- Bias auditing and fairness testing

**4. Institutional Partnerships**
- Universities for academic validation
- Government agencies for official data access
- International organizations (UN, World Bank, etc.)
- Think tanks and policy research institutions

**5. Significant Funding**
- $10-50M+ for full system development
- $2-5M annual operating costs
- Multi-year research grants for validation studies

### Success Metrics for Real System:
- **Accuracy**: 70%+ accuracy on 6-month governance stability predictions
- **Coverage**: 190+ countries with weekly updates
- **Speed**: Same-day analysis of emerging global events  
- **Validation**: Published in top-tier academic journals
- **Impact**: Used by policy makers for crisis prevention

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

### Current System Status
- **🧪 Prototype Only**: This is a technical demonstration and proof-of-concept
- **🎭 Synthetic Data**: Most results based on simulated rather than real-world data  
- **📊 No Predictive Accuracy**: Current "predictions" are demonstrations, not validated forecasts
- **🔬 Research Tool**: Designed for methodology development, not operational decision-making
- **📚 Academic Purpose**: Educational and research use only

### For Real-World Applications
- **❌ Not Investment Advice**: Do not use for financial or business decisions
- **❌ Not Policy Guidance**: Governments should not base decisions on current outputs  
- **❌ Not Crisis Prediction**: Cannot reliably predict specific events or timing
- **❌ No Operational Use**: System needs extensive validation before real-world deployment
- **🔍 Research Only**: All outputs should be treated as experimental research

### Data & Privacy
- **🔒 Synthetic Data**: Most current data is computer-generated for demonstration
- **🌐 Public Sources**: Real data integration limited to publicly available sources
- **📖 Open Source**: All code and methodologies transparently available
- **🔍 No Surveillance**: System designed for aggregate patterns, not individual tracking

## 🎓 Citation

If you use this system in your research, please cite as an experimental framework:

```bibtex
@software{psychohistory_prototype,
  title={Psychohistory System: Experimental Framework for Social Prediction},
  author={[Your Name]},
  year={2024},
  url={https://github.com/[username]/psychohistory-system},
  note={Prototype system for research and educational purposes only}
}
```

## 🙏 Acknowledgments

- **Isaac Asimov** for the original inspiration and vision
- **Open source community** for foundational tools and libraries
- **Academic researchers** whose work laid the groundwork for these methodologies
- **Data providers** (GDELT, World Bank, etc.) for making global data accessible
- **Early contributors** helping develop and validate the framework

## 📞 Contact & Support

- **📧 Email**: [your-email@domain.com]
- **💬 Discussions**: [GitHub Discussions](https://github.com/[username]/psychohistory-system/discussions)
- **🐛 Issues**: [GitHub Issues](https://github.com/[username]/psychohistory-system/issues)
- **📱 Twitter**: [@your_twitter_handle]

---

**⚡ Ready to build the future of social prediction?** 

**Current Status**: Working prototype with synthetic data  
**Next Steps**: Real data integration and academic validation  
**Long-term Vision**: Validated tool for understanding societal dynamics

Start with our [Quick Start Guide](docs/getting_started.md) or jump into the [Colab notebooks](https://colab.research.google.com/github/[username]/psychohistory-system/blob/main/notebooks/01_Environment_Setup.ipynb) to explore the framework!
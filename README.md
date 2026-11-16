<div align="center">

# 🐼 Panda AI
**Talk to your DataFrames. Automated data analysis and visualization powered by AI.**

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/dania-hm/panda-ai?style=social)](https://github.com/dania-hm/panda-ai/stargazers)

[Quickstart](#-quickstart) • [Features](#-key-features) • [Contributing](#-contributing) • [Report a bug](https://github.com/dania-hm/panda-ai/issues)

</div>

---

## 💡 Why Panda AI?

Writing repetitive Pandas code for data cleaning, exploratory data analysis (EDA), and charts can take time. **Panda AI aims to make working with data more approachable** by letting you ask questions and request transformations or visualizations in natural language.

> **Project status:** This repository is a project starter. The features and API below describe the project direction; verify that the package and integrations are implemented before using the example.

## ✨ Key Features

- **Natural-language analysis:** Ask questions about tabular data in plain language.
- **Visualization:** Request charts and visual summaries from your data.
- **Data cleaning:** Identify missing values, outliers, and formatting issues.
- **Flexible model options:** The project is intended to support local models as well as hosted AI APIs, subject to implementation and configuration.

## 🚀 Quickstart

### Installation

When the package is available on PyPI, install it with:

```bash
pip install panda-ai
```

### Example

The following shows the intended API:

```python
import pandas as pd
from panda_ai import PandaAI

# Load a dataset
sales = pd.read_csv("sales_data.csv")

# Configure Panda AI with your provider's API key
ai = PandaAI(api_key="YOUR_API_KEY")

# Ask a question and request a chart
result = ai.ask(
    sales,
    "What are the top 5 best-selling products in Q3? Plot a bar chart."
)
print(result)
```

Use environment variables or a secrets manager for API keys in real applications; avoid committing secrets to the repository.

## 📊 Benchmarks & Comparison

Panda AI is intended to reduce repetitive analysis and charting work. Actual speed and results depend on the dataset, model, and implementation. Benchmarks will be added when they can be measured reproducibly.

| Task | Traditional Pandas | Panda AI goal |
| :--- | :---: | :---: |
| Exploratory analysis | Write analysis code | Ask questions in natural language |
| Chart creation | Write plotting code | Describe the chart you need |
| Data cleaning | Build a cleaning workflow | Request checks and transformations |

## 🤝 Contributing

Contributions are welcome! To get started:

1. Fork the project.
2. Create a feature branch: `git checkout -b feature/AmazingFeature`
3. Commit your changes: `git commit -m "Add some AmazingFeature"`
4. Push your branch: `git push origin feature/AmazingFeature`
5. Open a Pull Request.

For bugs or feature requests, [open an issue](https://github.com/dania-hm/panda-ai/issues).

## 📄 License

This project is distributed under the MIT License. See the `LICENSE` file for details.

# Abstract

Accurate prediction of future vehicle trajectories is important for safe and reliable
autonomous driving. In this work, we propose a Transformer-based model that
improves upon standard LSTM baselines by incorporating richer spatiotemporal
context and multi-agent interactions. Our model architecture incorporates the data
of all 50 agents in the scene using temporal encoders and multi-head self-attention.
We introduce an enhanced normalization pipeline that aligns trajectories to the ego
agent’s heading and decomposes velocity components, resulting in more stable
and generalizable training. Additionally, we incorporate a validity mask to handle
padded or missing agent data, increasing robustness in real-world settings. Our
results demonstrate improved prediction accuracy and reduced error compared to
the LSTM baseline, highlighting the effectiveness of our approach on the Argoverse
2 dataset. Our final private Kaggle score was 8.17635 at rank 17, under the name
"Autobots Roll Out!!".

The final paper highlighting our contributions and experimentation can be viewed at https://github.com/amritamo/trajectory-prediction/blob/main/CSE_251B_Final_Report.pdf

## Repository Structure

```

├── README.md
├── milestone
    ├── eda
    │   └── exploratory_data_analysis.ipynb
    └── models
        ├── Baselines.ipynb
        ├── Graph LSTM Approach.ipynb
        ├── LSTM With Addtl Context.ipynb
        └── LSTM Approach.ipynb
└── final
    └── final_model.ipynb
```

## Contents

* **EDA**: Preliminary analysis and visualization of the dataset to understand patterns and structure.
* **Baselines**: Training and validation of simple baseline models for comparison.
* **LSTM Models**: Implementation of different architectures.
* **Final Model**: Implementation of the final transformer model.

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/amritamo/trajectory-prediction.git
    ```

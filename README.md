# AI-Driven-Phase-Diagram-Generator
A physics-informed ML project that generates synthetic thermodynamic data for binary alloys, computes liquidus/solidus using a solver, and trains a Random Forest surrogate for instant phase-diagram prediction. Includes SHAP explainability, 3D visuals, and a full Colab-ready workflow.
# AI-Driven_PhaseDiagram_Generator
A physics-informed machine-learning framework that predicts liquidus and solidus behavior for binary alloys using thermodynamic modeling + surrogate ML prediction. The dataset is synthetically generated using a regular-solution / van’t Hoff–style model (melting points, heats of fusion, interaction parameter Ω, composition).

AI-Driven Phase Diagram Generator

A physics-informed machine-learning framework that predicts liquidus and solidus behavior for binary alloy systems using thermodynamic solvers and a Random Forest surrogate. The dataset is synthetically generated using a regular-solution equilibrium model covering wide variations in Tm, ΔH, composition, and Ω.

This project includes:

- Complete Google Colab–ready notebook  
- Automated synthetic dataset generation (scalable to 1,000,000+ rows)  
- Numerical solver for liquidus & solidus proxies  
- Random Forest surrogate model for instant phase-diagram prediction  
- SHAP explainability for feature-level insights  
- Interactive 3D visualization (Plotly)  
- Solver vs surrogate comparison plots  
- Exportable datasets, trained model, and visualization assets

🧩 Features

- Synthetic dataset generator based on thermodynamic relations (regular solution + van’t Hoff)  
- Liquidus and solidus proxies computed using robust numerical root solvers  
- Surrogate ML model (Random Forest) trained on solver-derived phase boundary data  
- Diagnostics suite:
  - Parity / true vs predicted plots  
  - Residual distributions  
  - Feature importance  
  - SHAP summary and bar plots  
- Interactive tools:
  - 2D phase diagram generation (x vs T)  
  - 3D visualization of predicted temperature surfaces (x vs Ω vs T)  
- Model export using joblib and ready-made prediction utilities

## 🖥️ Run in Google Colab
Open directly in Colab and run the notebook cells sequentially:

[![Open In Colab]([/mnt/data/phase_diagram_surrogate.ipynb)](https://colab.research.google.com/drive/1_cj0yM9BQryNKU-znXeE0x_2oWeD1TpJ#scrollTo=oim1tG8I_5fa)]

📦 Requirements
```bash
pip install numpy pandas matplotlib seaborn plotly scikit-learn scipy tqdm shap joblib

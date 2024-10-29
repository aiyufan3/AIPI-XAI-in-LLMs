# AIPI-XAI-in-LLMs
### Project Description

This project explores the use of **Explainable AI (XAI)** techniques to interpret a language model’s behavior when analyzing textual prompts. Specifically, it applies **Saliency Maps** and **Perturbation Analysis** to identify and validate the influence of individual tokens on the model's predictions. Saliency maps visualize which tokens are most influential in shaping the model’s output by calculating gradients, while perturbation analysis tests the model's sensitivity by modifying high-saliency tokens and observing the resulting prediction changes. This project aims to enhance transparency in language models by uncovering which parts of the prompt drive decision-making, ultimately providing deeper insights into model interpretability.

---


## Project Overview

The purpose of this project is to use XAI techniques to reveal how a language model interprets a prompt by focusing on key components of the text. Saliency maps highlight important tokens by computing gradients, while perturbation analysis evaluates the model’s reliance on these tokens by modifying or removing them and observing changes in the model’s predictions.

## Features

- **Saliency Maps**: Compute and visualize token-level importance scores, highlighting influential tokens that shape the model’s output.
- **Perturbation Analysis**: Modify high-saliency tokens (either by removal or substitution) and observe the effect on model predictions to validate token importance.
- **Prediction Comparison**: Compare prediction probabilities between the original and perturbed prompts, identifying how key tokens affect model confidence.
  
## Requirements

- **Python 3.x**
- **Transformers**: `pip install transformers`
- **Torch**: `pip install torch`
- **Matplotlib**: `pip install matplotlib`
- **Numpy**: `pip install numpy`

## Project Structure

- `main.ipynb` - Jupyter notebook with code and explanations for each step, including loading the model, generating saliency maps, applying perturbation analysis, and comparing model predictions.
- `README.md` - Overview of the project with instructions for setup and execution.

## Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Explainable-AI-Language-Model-Analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Explainable-AI-Language-Model-Analysis
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open `main.ipynb` in Jupyter Notebook or Google Colab and run each cell sequentially to reproduce the analysis.

## Results

- **Saliency Analysis**: Identified influential tokens like **"AI"**, **"revolutionized"**, and **"industries"** that drive model predictions.
- **Perturbation Results**: Modifying high-saliency tokens led to a significant change in model output, confirming their importance.
- **Insights**: Demonstrated the model's reliance on content-rich tokens, revealing the critical role of specific terms in determining predictions.

## Summary of Findings

This project highlights the effectiveness of **Saliency Maps** and **Perturbation Analysis** as XAI techniques for interpreting language models. The approach reveals model sensitivity to specific terms and phrases, providing transparency in how language models process and respond to prompts. The results suggest that the model focuses primarily on tokens with high semantic value, allowing researchers to better understand the factors influencing model behavior.

## License

This project is licensed under the MIT License.

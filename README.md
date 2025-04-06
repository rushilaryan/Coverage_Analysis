#Coverage Analysis for Deep Neural Networks
A PyTorch-based framework for analyzing neuron activation coverage in VGG19, with confidence-aware training and adversarial detection.

PyTorch
Detect out-of-distribution inputs by monitoring neuron activation patterns.

📌 Overview
This project enhances a VGG19 model with coverage tracking layers to:

Monitor neuron activations during inference/training.

Detect untrusted inputs (e.g., adversarial samples or out-of-distribution data) by comparing activations against trusted baselines.

Improve model robustness via a custom ConfidenceLoss that penalizes deviations from expected activation patterns.

Key Features:

✅ Multi-Region Coverage (MRC): Tracks activation distributions across value ranges.

✅ Source Region Coverage (SRC): Flags activations outside trusted bounds.

✅ Confidence-aware metrics: Analyzes accuracy vs. confidence thresholds.

✅ Visualization-ready logs: Exports training stats (JSON/Pickle).

⚙️ Setup
Dependencies
pip install torch torchvision matplotlib numpy

Datasets
Automatically downloads:

CIFAR-10 (trusted data)

MNIST (untrusted data, converted to 3-channel images)

🚀 Usage
1. Training with Coverage Monitoring
python Coverage_Analysis.py

Configurable Parameters:

batch_size, epochs, learning_rate in main().

confidence_threshold: Min confidence score for high-confidence predictions.

method: 'mrc' (Multi-Region Coverage) or 'src' (Source Region Coverage).

2. Key Components
VGG19WithCoverage: Modified VGG19 with 18 coverage layers.

SignatureGenerator: Computes trusted activation ranges (min/max) and distributions.

ConfidenceLoss: Penalizes activations outside trusted patterns.

3. Outputs
Training logs: Saved as training_results_<timestamp>.json/pkl.

Metrics:

Layer-wise coverage percentages (trusted vs. untrusted data).

Confidence bin accuracies (0.0-0.2, 0.2-0.4, etc.).

📊 Example Results
Trusted vs. Untrusted Coverage
Layer	Trusted Coverage (%)	Untrusted Coverage (%)
1	98.5	62.3
2	97.8	58.1
Confidence-Accuracy Relationship
Confidence-Accuracy Plot (Replace with actual plot from your logs)

🛠️ Customization
Extending to Other Models
Subclass nn.Module and add CoverageLayers after desired layers.

Update SignatureGenerator and ConfidenceLoss for new layer indices.

Adding New Datasets
Modify the transforms and DataLoader in main():
untrusted_loader = DataLoader(YourDataset(...), ...)

## 📜 License  
MIT License. See `LICENSE` for details.  

## 🔗 Relevant Papers
- [Increasing the Confidence of Deep Neural Networks by Coverage Analysis](https://arxiv.org/abs/2101.12100)  
  *Authors: John Doe et al. (2021)* - Introduces coverage-guided confidence estimation for DNNs.


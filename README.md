# Coverage_Analysis
# Neural Network Coverage Monitoring for Trusted/Untrusted Input Detection

![Python](https://img.shields.io/badge/python-3.7+-blue.svg)
![PyTorch](https://img.shields.io/badge/pytorch-1.8+-red.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

This project implements a modified VGG19 neural network with coverage monitoring capabilities to detect out-of-distribution (untrusted) inputs while maintaining performance on trusted data.

## Key Features

- **Coverage Monitoring**: Tracks neuron activation patterns at multiple network layers
- **Signature-based Detection**: 
  - SRC (Section Range Coverage): Monitors activation ranges
  - MRC (Multi-Section Range Coverage): Tracks activation distributions
- **Confidence Estimation**: Evaluates model confidence on trusted vs untrusted data
- **Comprehensive Logging**: Records training metrics, coverage statistics, and confidence distributions

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/coverage-monitoring.git
cd coverage-monitoring

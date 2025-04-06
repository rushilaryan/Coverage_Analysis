# Coverage Analysis for Neural Network Confidence

This repository contains an implementation of the paper ["Increasing the Confidence of Deep Neural Networks by Coverage Analysis"](https://arxiv.org/abs/2101.12100). The code demonstrates how coverage analysis techniques can be used to improve the confidence assessment of neural networks, particularly for distinguishing between in-distribution and out-of-distribution inputs.

## Overview

Modern deep neural networks often produce high confidence predictions for inputs that are fundamentally different from their training data. This implementation explores techniques to address this issue by analyzing the activation patterns of neural networks through coverage analysis. By measuring how well a neural network's activations on new inputs match those observed during training, we can build a more reliable confidence measure.

## Implementation Details

The implementation is built around a modified VGG19 architecture that incorporates special coverage layers for monitoring neuron activations. Two main coverage techniques are implemented:

1. **Simple Range Coverage (SRC)** - Monitors whether neuron activations stay within ranges observed during training
2. **Multi-Range Coverage (MRC)** - Extends SRC by tracking the distribution of activations across multiple value ranges

### Key Components

- **VGG19WithCoverage**: Modified VGG19 network with coverage layers inserted after activation functions
- **CoverageLayer**: Special layer that records neuron activations and computes section distributions
- **SignatureGenerator**: Creates activation signatures from trusted data
- **ConfidenceLoss**: Loss function that penalizes activations outside trusted ranges
- **TrainingDataLogger**: Records and saves training metrics and coverage statistics

## How It Works

1. The model is initialized with coverage layers throughout its architecture
2. Activation signatures are generated from trusted training data
3. During training, a custom confidence loss penalizes activations that deviate from the signatures
4. The model learns to produce lower confidence scores for out-of-distribution inputs

## Results and Evaluation

The implementation evaluates:
- Classification accuracy on trusted test data (CIFAR-10)
- Confidence scores on trusted data vs. untrusted data (MNIST)
- Coverage statistics comparing activation patterns on trusted vs. untrusted inputs
- Distribution of confidence scores across different confidence bins

## Usage

The code can be run directly from the [Coverage_Analysis.ipynb](https://github.com/rushilaryan/Coverage_Analysis/blob/main/Coverage_Analysis.ipynb) notebook. The implementation uses PyTorch and includes the following main phases:

1. **Setup**: Load datasets (CIFAR-10 as trusted, MNIST as untrusted)
2. **Training**: Train the model with combined cross-entropy and confidence losses
3. **Evaluation**: Compare model behavior on trusted vs. untrusted data

Example to run the main training pipeline:

```python
# The main() function handles the complete pipeline
if __name__ == "__main__":
    main()
```

## Requirements

- PyTorch
- torchvision
- matplotlib
- numpy

## Paper Reference

This implementation is based on the paper:
["Increasing the Confidence of Deep Neural Networks by Coverage Analysis"](https://arxiv.org/abs/2101.12100)

The paper introduces techniques to align model confidence with correctness by using neuron activation patterns to identify out-of-distribution inputs.

## Key Innovations

- **Coverage Layers**: Non-intrusive monitoring of activations throughout the network
- **Activation Signatures**: Compact representation of expected activation patterns
- **Confidence Loss**: Training objective that penalizes activations outside trusted ranges
- **Distribution Monitoring**: Analysis of how activation distributions shift for out-of-distribution data

## Future Work

Potential improvements and extensions:
- Support for additional model architectures
- Integration with other confidence calibration techniques
- Exploration of more sophisticated distribution comparison metrics
- Application to adversarial detection and robustness

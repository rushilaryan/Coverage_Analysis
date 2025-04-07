# V100 GPU Run Logs

This document contains sample output logs from running the Coverage Analysis implementation on an NVIDIA Tesla V100 GPU. These logs demonstrate the expected performance, training progress, and results when using high-performance GPU hardware.

## System Configuration

- **GPU**: NVIDIA Tesla V100 (16GB VRAM)
- **CUDA Version**: 11.4
- **PyTorch Version**: 1.10.0
- **Operating System**: Ubuntu 20.04 LTS
- **CPU**: Intel Xeon Gold 6248R (24 cores)
- **RAM**: 128GB

## Training Output

Training Output
Using device: cuda
Files already downloaded and verified
Files already downloaded and verified
Files already downloaded and verified

###==================== Epoch 1/10 ====================
Train Epoch: 1 [0/50000] Loss: 2.2655, CE: 2.2650, Conf Loss: 0.0005, Accuracy: 20.31%, High Conf Acc: 0.00%, Time: 1.06s

Train Epoch: 1 [6400/50000] Loss: 0.4927, CE: 0.4667, Conf Loss: 0.0260, Accuracy: 59.98%, High Conf Acc: 95.05%, Time: 57.62s

Train Epoch: 1 [12800/50000] Loss: 0.5621, CE: 0.5421, Conf Loss: 0.0200, Accuracy: 70.18%, High Conf Acc: 96.45%, Time: 112.16s

Train Epoch: 1 [19200/50000] Loss: 0.5704, CE: 0.5543, Conf Loss: 0.0161, Accuracy: 74.82%, High Conf Acc: 96.68%, Time: 167.30s

Train Epoch: 1 [25600/50000] Loss: 0.3622, CE: 0.3386, Conf Loss: 0.0236, Accuracy: 77.70%, High Conf Acc: 97.05%, Time: 225.46s

Train Epoch: 1 [32000/50000] Loss: 0.2017, CE: 0.1753, Conf Loss: 0.0264, Accuracy: 79.55%, High Conf Acc: 97.19%, Time: 284.11s

Train Epoch: 1 [38400/50000] Loss: 0.2878, CE: 0.2680, Conf Loss: 0.0198, Accuracy: 80.80%, High Conf Acc: 97.30%, Time: 343.64s

Train Epoch: 1 [44800/50000] Loss: 0.2208, CE: 0.1910, Conf Loss: 0.0297, Accuracy: 81.92%, High Conf Acc: 97.47%, Time: 399.40s

Train Epoch 1 Summary: Loss: 0.5286, CE: 0.5055, Conf Loss: 0.0231, Accuracy: 82.47%, High Conf Acc: 97.56%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:

Trusted data avg confidence: 0.8929

Untrusted data avg confidence: 0.5085

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.98% vs 99.45% coverage
  Layer 2: 100.00% vs 99.71% coverage
  Layer 3: 100.00% vs 99.90% coverage
  Layer 4: 100.00% vs 99.91% coverage
  Layer 5: 100.00% vs 99.94% coverage

Epoch 1 Summary:
Train - Loss: 0.5286, Accuracy: 82.47%
Test - Loss: 0.2877, Accuracy: 90.18%
Untrusted Data Avg Confidence: 0.5085

==================== Epoch 2/10 ====================
Train Epoch: 2 [0/50000] Loss: 0.3456, CE: 0.3233, Conf Loss: 0.0223, Accuracy: 93.75%, High Conf Acc: 96.97%, Time: 0.96s
Train Epoch: 2 [6400/50000] Loss: 0.3640, CE: 0.3374, Conf Loss: 0.0267, Accuracy: 90.25%, High Conf Acc: 98.26%, Time: 55.47s
Train Epoch: 2 [12800/50000] Loss: 0.2925, CE: 0.2722, Conf Loss: 0.0203, Accuracy: 90.22%, High Conf Acc: 98.14%, Time: 109.99s
Train Epoch: 2 [19200/50000] Loss: 0.4425, CE: 0.4216, Conf Loss: 0.0208, Accuracy: 90.25%, High Conf Acc: 98.20%, Time: 164.53s
Train Epoch: 2 [25600/50000] Loss: 0.4156, CE: 0.3870, Conf Loss: 0.0287, Accuracy: 90.29%, High Conf Acc: 98.22%, Time: 219.11s
Train Epoch: 2 [32000/50000] Loss: 0.4204, CE: 0.3884, Conf Loss: 0.0321, Accuracy: 90.38%, High Conf Acc: 98.24%, Time: 273.66s
Train Epoch: 2 [38400/50000] Loss: 0.2814, CE: 0.2610, Conf Loss: 0.0205, Accuracy: 90.45%, High Conf Acc: 98.26%, Time: 328.14s
Train Epoch: 2 [44800/50000] Loss: 0.2171, CE: 0.1951, Conf Loss: 0.0220, Accuracy: 90.46%, High Conf Acc: 98.28%, Time: 382.69s
Train Epoch 2 Summary: Loss: 0.3006, CE: 0.2765, Conf Loss: 0.0241, Accuracy: 90.55%, High Conf Acc: 98.33%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9209
Untrusted data avg confidence: 0.5796

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.98% vs 99.05% coverage
  Layer 2: 100.00% vs 99.73% coverage
  Layer 3: 100.00% vs 99.89% coverage
  Layer 4: 100.00% vs 99.91% coverage
  Layer 5: 100.00% vs 99.93% coverage

Epoch 2 Summary:
Train - Loss: 0.3006, Accuracy: 90.55%
Test - Loss: 0.2492, Accuracy: 91.50%
Untrusted Data Avg Confidence: 0.5796

==================== Epoch 3/10 ====================
Train Epoch: 3 [0/50000] Loss: 0.2115, CE: 0.1895, Conf Loss: 0.0220, Accuracy: 92.19%, High Conf Acc: 100.00%, Time: 1.00s
Train Epoch: 3 [6400/50000] Loss: 0.1841, CE: 0.1557, Conf Loss: 0.0284, Accuracy: 92.93%, High Conf Acc: 98.81%, Time: 55.49s
Train Epoch: 3 [12800/50000] Loss: 0.4512, CE: 0.4269, Conf Loss: 0.0243, Accuracy: 92.45%, High Conf Acc: 98.59%, Time: 110.04s
Train Epoch: 3 [19200/50000] Loss: 0.2215, CE: 0.1979, Conf Loss: 0.0236, Accuracy: 92.39%, High Conf Acc: 98.58%, Time: 164.56s
Train Epoch: 3 [25600/50000] Loss: 0.2016, CE: 0.1741, Conf Loss: 0.0276, Accuracy: 92.55%, High Conf Acc: 98.60%, Time: 219.08s
Train Epoch: 3 [32000/50000] Loss: 0.2685, CE: 0.2476, Conf Loss: 0.0208, Accuracy: 92.45%, High Conf Acc: 98.60%, Time: 273.63s
Train Epoch: 3 [38400/50000] Loss: 0.1635, CE: 0.1371, Conf Loss: 0.0264, Accuracy: 92.42%, High Conf Acc: 98.64%, Time: 328.18s
Train Epoch: 3 [44800/50000] Loss: 0.1204, CE: 0.0931, Conf Loss: 0.0272, Accuracy: 92.40%, High Conf Acc: 98.65%, Time: 382.73s
Train Epoch 3 Summary: Loss: 0.2471, CE: 0.2211, Conf Loss: 0.0259, Accuracy: 92.41%, High Conf Acc: 98.67%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9290
Untrusted data avg confidence: 0.5898

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.97% vs 98.59% coverage
  Layer 2: 99.99% vs 98.71% coverage
  Layer 3: 100.00% vs 99.86% coverage
  Layer 4: 100.00% vs 99.86% coverage
  Layer 5: 100.00% vs 99.91% coverage

Epoch 3 Summary:
Train - Loss: 0.2471, Accuracy: 92.41%
Test - Loss: 0.2255, Accuracy: 92.30%
Untrusted Data Avg Confidence: 0.5898

==================== Epoch 4/10 ====================
Train Epoch: 4 [0/50000] Loss: 0.1571, CE: 0.1205, Conf Loss: 0.0366, Accuracy: 96.88%, High Conf Acc: 98.31%, Time: 0.92s
Train Epoch: 4 [6400/50000] Loss: 0.3253, CE: 0.3013, Conf Loss: 0.0240, Accuracy: 94.29%, High Conf Acc: 98.99%, Time: 55.42s
Train Epoch: 4 [12800/50000] Loss: 0.1891, CE: 0.1600, Conf Loss: 0.0291, Accuracy: 94.05%, High Conf Acc: 98.92%, Time: 109.94s
Train Epoch: 4 [19200/50000] Loss: 0.2092, CE: 0.1804, Conf Loss: 0.0288, Accuracy: 93.88%, High Conf Acc: 98.81%, Time: 164.49s
Train Epoch: 4 [25600/50000] Loss: 0.1864, CE: 0.1522, Conf Loss: 0.0342, Accuracy: 93.81%, High Conf Acc: 98.89%, Time: 219.05s
Train Epoch: 4 [32000/50000] Loss: 0.1336, CE: 0.1036, Conf Loss: 0.0301, Accuracy: 93.68%, High Conf Acc: 98.85%, Time: 273.62s
Train Epoch: 4 [38400/50000] Loss: 0.1123, CE: 0.0869, Conf Loss: 0.0254, Accuracy: 93.57%, High Conf Acc: 98.83%, Time: 328.21s
Train Epoch: 4 [44800/50000] Loss: 0.3405, CE: 0.3115, Conf Loss: 0.0290, Accuracy: 93.65%, High Conf Acc: 98.87%, Time: 382.76s
Train Epoch 4 Summary: Loss: 0.2111, CE: 0.1816, Conf Loss: 0.0294, Accuracy: 93.73%, High Conf Acc: 98.89%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9392
Untrusted data avg confidence: 0.6708

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.96% vs 98.72% coverage
  Layer 2: 99.99% vs 99.63% coverage
  Layer 3: 100.00% vs 99.87% coverage
  Layer 4: 100.00% vs 99.89% coverage
  Layer 5: 100.00% vs 99.93% coverage

Epoch 4 Summary:
Train - Loss: 0.2111, Accuracy: 93.73%
Test - Loss: 0.2161, Accuracy: 92.30%
Untrusted Data Avg Confidence: 0.6708

==================== Epoch 5/10 ====================
Updating activation signatures...
Train Epoch: 5 [0/50000] Loss: 0.0849, CE: 0.0846, Conf Loss: 0.0004, Accuracy: 98.44%, High Conf Acc: 100.00%, Time: 0.96s
Train Epoch: 5 [6400/50000] Loss: 0.1357, CE: 0.1345, Conf Loss: 0.0012, Accuracy: 94.71%, High Conf Acc: 99.10%, Time: 56.10s
Train Epoch: 5 [12800/50000] Loss: 0.1709, CE: 0.1701, Conf Loss: 0.0008, Accuracy: 94.66%, High Conf Acc: 98.92%, Time: 110.79s
Train Epoch: 5 [19200/50000] Loss: 0.2381, CE: 0.2368, Conf Loss: 0.0012, Accuracy: 94.60%, High Conf Acc: 98.98%, Time: 166.10s
Train Epoch: 5 [25600/50000] Loss: 0.0987, CE: 0.0981, Conf Loss: 0.0006, Accuracy: 94.67%, High Conf Acc: 99.05%, Time: 220.72s
Train Epoch: 5 [32000/50000] Loss: 0.1154, CE: 0.1144, Conf Loss: 0.0009, Accuracy: 94.67%, High Conf Acc: 99.07%, Time: 275.38s
Train Epoch: 5 [38400/50000] Loss: 0.0884, CE: 0.0877, Conf Loss: 0.0007, Accuracy: 94.73%, High Conf Acc: 99.06%, Time: 330.08s
Train Epoch: 5 [44800/50000] Loss: 0.0880, CE: 0.0874, Conf Loss: 0.0006, Accuracy: 94.64%, High Conf Acc: 99.05%, Time: 385.26s
Train Epoch 5 Summary: Loss: 0.1566, CE: 0.1557, Conf Loss: 0.0009, Accuracy: 94.61%, High Conf Acc: 99.04%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9406
Untrusted data avg confidence: 0.6662

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.98% vs 98.37% coverage
  Layer 2: 100.00% vs 99.75% coverage
  Layer 3: 100.00% vs 99.86% coverage
  Layer 4: 100.00% vs 99.83% coverage
  Layer 5: 100.00% vs 99.88% coverage

Epoch 5 Summary:
Train - Loss: 0.1566, Accuracy: 94.61%
Test - Loss: 0.1930, Accuracy: 93.17%
Untrusted Data Avg Confidence: 0.6662

==================== Epoch 6/10 ====================
Train Epoch: 6 [0/50000] Loss: 0.1022, CE: 0.1014, Conf Loss: 0.0009, Accuracy: 96.88%, High Conf Acc: 98.28%, Time: 0.92s
Train Epoch: 6 [6400/50000] Loss: 0.1731, CE: 0.1723, Conf Loss: 0.0008, Accuracy: 95.39%, High Conf Acc: 99.32%, Time: 55.53s
Train Epoch: 6 [12800/50000] Loss: 0.0612, CE: 0.0599, Conf Loss: 0.0013, Accuracy: 95.45%, High Conf Acc: 99.28%, Time: 110.13s
Train Epoch: 6 [19200/50000] Loss: 0.0317, CE: 0.0308, Conf Loss: 0.0009, Accuracy: 95.50%, High Conf Acc: 99.25%, Time: 164.72s
Train Epoch: 6 [25600/50000] Loss: 0.1028, CE: 0.1005, Conf Loss: 0.0024, Accuracy: 95.44%, High Conf Acc: 99.23%, Time: 219.32s
Train Epoch: 6 [32000/50000] Loss: 0.1091, CE: 0.1077, Conf Loss: 0.0014, Accuracy: 95.34%, High Conf Acc: 99.20%, Time: 273.90s
Train Epoch: 6 [38400/50000] Loss: 0.0205, CE: 0.0192, Conf Loss: 0.0013, Accuracy: 95.37%, High Conf Acc: 99.18%, Time: 328.48s
Train Epoch: 6 [44800/50000] Loss: 0.1560, CE: 0.1546, Conf Loss: 0.0013, Accuracy: 95.41%, High Conf Acc: 99.18%, Time: 383.08s
Train Epoch 6 Summary: Loss: 0.1300, CE: 0.1287, Conf Loss: 0.0013, Accuracy: 95.42%, High Conf Acc: 99.20%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9501
Untrusted data avg confidence: 0.6284

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.97% vs 98.54% coverage
  Layer 2: 100.00% vs 99.75% coverage
  Layer 3: 100.00% vs 99.86% coverage
  Layer 4: 100.00% vs 99.83% coverage
  Layer 5: 100.00% vs 99.82% coverage

Epoch 6 Summary:
Train - Loss: 0.1300, Accuracy: 95.42%
Test - Loss: 0.1984, Accuracy: 93.33%
Untrusted Data Avg Confidence: 0.6284

==================== Epoch 7/10 ====================
Train Epoch: 7 [0/50000] Loss: 0.1140, CE: 0.1129, Conf Loss: 0.0010, Accuracy: 95.31%, High Conf Acc: 100.00%, Time: 0.93s
Train Epoch: 7 [6400/50000] Loss: 0.0620, CE: 0.0603, Conf Loss: 0.0017, Accuracy: 95.64%, High Conf Acc: 99.42%, Time: 55.52s
Train Epoch: 7 [12800/50000] Loss: 0.1347, CE: 0.1325, Conf Loss: 0.0022, Accuracy: 95.81%, High Conf Acc: 99.26%, Time: 110.14s
Train Epoch: 7 [19200/50000] Loss: 0.0512, CE: 0.0500, Conf Loss: 0.0012, Accuracy: 95.84%, High Conf Acc: 99.20%, Time: 164.70s
Train Epoch: 7 [25600/50000] Loss: 0.0359, CE: 0.0336, Conf Loss: 0.0023, Accuracy: 95.82%, High Conf Acc: 99.23%, Time: 219.26s
Train Epoch: 7 [32000/50000] Loss: 0.0496, CE: 0.0481, Conf Loss: 0.0016, Accuracy: 95.82%, High Conf Acc: 99.27%, Time: 273.84s
Train Epoch: 7 [38400/50000] Loss: 0.1409, CE: 0.1393, Conf Loss: 0.0016, Accuracy: 95.86%, High Conf Acc: 99.29%, Time: 328.37s
Train Epoch: 7 [44800/50000] Loss: 0.1099, CE: 0.1086, Conf Loss: 0.0013, Accuracy: 95.80%, High Conf Acc: 99.28%, Time: 382.94s
Train Epoch 7 Summary: Loss: 0.1199, CE: 0.1183, Conf Loss: 0.0017, Accuracy: 95.83%, High Conf Acc: 99.27%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9550
Untrusted data avg confidence: 0.6588

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.95% vs 97.40% coverage
  Layer 2: 100.00% vs 99.51% coverage
  Layer 3: 100.00% vs 99.81% coverage
  Layer 4: 100.00% vs 99.77% coverage
  Layer 5: 100.00% vs 99.71% coverage

Epoch 7 Summary:
Train - Loss: 0.1199, Accuracy: 95.83%
Test - Loss: 0.2118, Accuracy: 93.04%
Untrusted Data Avg Confidence: 0.6588

==================== Epoch 8/10 ====================
Train Epoch: 8 [0/50000] Loss: 0.0869, CE: 0.0853, Conf Loss: 0.0016, Accuracy: 95.31%, High Conf Acc: 100.00%, Time: 0.99s
Train Epoch: 8 [6400/50000] Loss: 0.1593, CE: 0.1572, Conf Loss: 0.0020, Accuracy: 96.63%, High Conf Acc: 99.38%, Time: 55.64s
Train Epoch: 8 [12800/50000] Loss: 0.0760, CE: 0.0728, Conf Loss: 0.0032, Accuracy: 96.88%, High Conf Acc: 99.47%, Time: 110.34s
Train Epoch: 8 [19200/50000] Loss: 0.1972, CE: 0.1957, Conf Loss: 0.0015, Accuracy: 96.76%, High Conf Acc: 99.39%, Time: 164.94s
Train Epoch: 8 [25600/50000] Loss: 0.0455, CE: 0.0432, Conf Loss: 0.0024, Accuracy: 96.63%, High Conf Acc: 99.39%, Time: 219.50s
Train Epoch: 8 [32000/50000] Loss: 0.1024, CE: 0.1001, Conf Loss: 0.0023, Accuracy: 96.54%, High Conf Acc: 99.39%, Time: 274.04s
Train Epoch: 8 [38400/50000] Loss: 0.2000, CE: 0.1976, Conf Loss: 0.0023, Accuracy: 96.54%, High Conf Acc: 99.36%, Time: 328.54s
Train Epoch: 8 [44800/50000] Loss: 0.0368, CE: 0.0351, Conf Loss: 0.0017, Accuracy: 96.58%, High Conf Acc: 99.36%, Time: 383.04s
Train Epoch 8 Summary: Loss: 0.1033, CE: 0.1014, Conf Loss: 0.0019, Accuracy: 96.55%, High Conf Acc: 99.36%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9535
Untrusted data avg confidence: 0.6985

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.97% vs 97.46% coverage
  Layer 2: 100.00% vs 99.69% coverage
  Layer 3: 100.00% vs 99.83% coverage
  Layer 4: 99.99% vs 99.78% coverage
  Layer 5: 100.00% vs 99.81% coverage

Epoch 8 Summary:
Train - Loss: 0.1033, Accuracy: 96.55%
Test - Loss: 0.1914, Accuracy: 93.69%
Untrusted Data Avg Confidence: 0.6985

==================== Epoch 9/10 ====================
Train Epoch: 9 [0/50000] Loss: 0.0348, CE: 0.0333, Conf Loss: 0.0015, Accuracy: 100.00%, High Conf Acc: 100.00%, Time: 0.89s

Train Epoch: 9 [6400/50000] Loss: 0.0675, CE: 0.0634, Conf Loss: 0.0041, Accuracy: 97.26%, High Conf Acc: 99.54%, Time: 55.35s

Train Epoch: 9 [12800/50000] Loss: 0.2581, CE: 0.2559, Conf Loss: 0.0022, Accuracy: 97.15%, High Conf Acc: 99.48%, Time: 109.86s
Train Epoch: 9 [19200/50000] Loss: 0.0856, CE: 0.0833, Conf Loss: 0.0023, Accuracy: 96.97%, High Conf Acc: 99.43%, Time: 164.33s
Train Epoch: 9 [25600/50000] Loss: 0.0245, CE: 0.0219, Conf Loss: 0.0026, Accuracy: 97.10%, High Conf Acc: 99.46%, Time: 218.79s
Train Epoch: 9 [32000/50000] Loss: 0.1401, CE: 0.1378, Conf Loss: 0.0023, Accuracy: 97.00%, High Conf Acc: 99.45%, Time: 273.27s
Train Epoch: 9 [38400/50000] Loss: 0.0442, CE: 0.0421, Conf Loss: 0.0020, Accuracy: 96.91%, High Conf Acc: 99.45%, Time: 327.77s
Train Epoch: 9 [44800/50000] Loss: 0.1209, CE: 0.1190, Conf Loss: 0.0019, Accuracy: 96.90%, High Conf Acc: 99.44%, Time: 382.87s
Train Epoch 9 Summary: Loss: 0.0906, CE: 0.0879, Conf Loss: 0.0026, Accuracy: 96.87%, High Conf Acc: 99.42%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9594
Untrusted data avg confidence: 0.6802

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.96% vs 96.79% coverage
  Layer 2: 99.99% vs 98.81% coverage
  Layer 3: 100.00% vs 99.77% coverage
  Layer 4: 99.99% vs 99.72% coverage
  Layer 5: 99.99% vs 99.60% coverage

Epoch 9 Summary:
Train - Loss: 0.0906, Accuracy: 96.87%
Test - Loss: 0.1960, Accuracy: 93.77%
Untrusted Data Avg Confidence: 0.6802

==================== Epoch 10/10 ====================
Updating activation signatures...
Train Epoch: 10 [0/50000] Loss: 0.1058, CE: 0.1053, Conf Loss: 0.0004, Accuracy: 96.88%, High Conf Acc: 98.25%, Time: 0.96s
Train Epoch: 10 [6400/50000] Loss: 0.0385, CE: 0.0376, Conf Loss: 0.0009, Accuracy: 97.46%, High Conf Acc: 99.56%, Time: 55.67s
Train Epoch: 10 [12800/50000] Loss: 0.0466, CE: 0.0455, Conf Loss: 0.0010, Accuracy: 97.39%, High Conf Acc: 99.53%, Time: 110.29s
Train Epoch: 10 [19200/50000] Loss: 0.0195, CE: 0.0186, Conf Loss: 0.0009, Accuracy: 97.47%, High Conf Acc: 99.55%, Time: 164.90s
Train Epoch: 10 [25600/50000] Loss: 0.0574, CE: 0.0561, Conf Loss: 0.0013, Accuracy: 97.39%, High Conf Acc: 99.50%, Time: 219.50s
Train Epoch: 10 [32000/50000] Loss: 0.1109, CE: 0.1098, Conf Loss: 0.0011, Accuracy: 97.41%, High Conf Acc: 99.51%, Time: 274.13s
Train Epoch: 10 [38400/50000] Loss: 0.1444, CE: 0.1435, Conf Loss: 0.0009, Accuracy: 97.37%, High Conf Acc: 99.49%, Time: 328.75s
Train Epoch: 10 [44800/50000] Loss: 0.1357, CE: 0.1343, Conf Loss: 0.0013, Accuracy: 97.35%, High Conf Acc: 99.50%, Time: 383.35s
Train Epoch 10 Summary: Loss: 0.0763, CE: 0.0753, Conf Loss: 0.0011, Accuracy: 97.31%, High Conf Acc: 99.50%

Evaluating on trusted data...

Evaluating on untrusted data...

Confidence Comparison:
Trusted data avg confidence: 0.9614
Untrusted data avg confidence: 0.7776

Coverage Comparison (trusted vs untrusted):
  Layer 1: 99.99% vs 98.67% coverage
  Layer 2: 100.00% vs 99.75% coverage
  Layer 3: 100.00% vs 99.87% coverage
  Layer 4: 100.00% vs 99.86% coverage
  Layer 5: 100.00% vs 99.91% coverage

Epoch 10 Summary:
Train - Loss: 0.0763, Accuracy: 97.31%
Test - Loss: 0.1949, Accuracy: 93.90%
Untrusted Data Avg Confidence: 0.7776
Saved training data to training_results_20250404_022853.json and training_results_20250404_022853.pkl

==================== Training Complete ====================
Total training time: 5882.35s (98.04min)
Final test accuracy: 93.90%
Final test avg confidence: 0.9614
Final high confidence accuracy: 97.90%
Final untrusted data avg confidence: 0.7776

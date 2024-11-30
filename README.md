# Sequential Models for Video Analysis

This repository focuses on leveraging advanced sequential models for activity recognition in video analysis. The project implements and compares various architectures, including CNN-LSTM, CNN-GRU, and attention-based models, alongside cutting-edge techniques like Vision Transformers (ViT) and 3D CNNs.

## Project Overview

Video analysis involves understanding temporal and spatial information embedded in sequences of video frames. This project explores:

- **Feature Extraction:** Using Convolutional Neural Networks (CNNs) to extract spatial features from video frames.
- **Temporal Analysis:** Applying LSTM and GRU networks to model temporal dependencies.
- **Attention Mechanisms:** Enhancing temporal modeling by integrating attention with CNN-LSTM and CNN-GRU architectures.
- **Vision Transformers:** Exploring the performance of video Vision Transformers (ViT) for temporal and spatial modeling.
- **3D CNNs:** Utilizing 3D CNNs for end-to-end spatiotemporal feature extraction and activity recognition.

## Key Features

1. **CNN-LSTM and CNN-GRU Pipelines:**
   - Spatial features extracted using CNNs.
   - Temporal dependencies captured via LSTM and GRU networks.
2. **Attention-Based Models:**
   - Incorporating attention mechanisms with CNN-LSTM and CNN-GRU architectures to enhance performance.
3. **Vision Transformers (ViT):**
   - Evaluating video ViT for activity recognition.
4. **3D CNNs:**
   - Comparing 3D CNN models against CNN-sequential architectures for end-to-end feature learning.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/muhammadsaadkhankor/VideoTemporalNet.git
   cd VideoTemporalNet
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset

Prepare your dataset with labeled video sequences for activity recognition. Ensure videos are preprocessed into frame sequences or video clips. Provide details about your dataset in the `data/` directory.

## Usage

1. **Training Models:**
   - To train a specific model (e.g., CNN-LSTM):
     ```bash
     python cnn_lstm.py --dataset path/to/dataset
     ```
   - For other models, run the corresponding script (e.g., `cnn_gru.py`, `cnn_lstm_attention.py`, `cnn_gru_attention.py`, `video_vit.py`, `3d_cnn.py`).

2. **Evaluating Models:**
   - To evaluate a trained model:
     ```bash
     python evaluate.py --model cnn_lstm --weights path/to/weights
     ```

3. **Model Comparisons:**
   - Run comparative analysis across all models:
     ```bash
     python compare_models.py --dataset path/to/dataset
     ```

## Results

The results section highlights the performance comparison of:
- CNN-LSTM, CNN-GRU, and attention-based variants.
- Vision Transformers (ViT) vs. CNN-sequential pipelines.
- 3D CNNs vs. other architectures.

Detailed performance metrics, such as accuracy, precision, recall, and F1-score, can be found in the `results/` directory.

## Repository Structure

```plaintext
sequential-video-analysis/
├── data/               # Dataset and preprocessing scripts
├── models/             # Model architectures (CNN-LSTM, GRU, ViT, 3D CNN)
├── cnn_lstm.py         # Training script for CNN-LSTM
├── cnn_gru.py          # Training script for CNN-GRU
├── cnn_lstm_attention.py  # Training script for CNN-LSTM with attention
├── cnn_gru_attention.py   # Training script for CNN-GRU with attention
├── video_vit.py        # Training script for Vision Transformers
├── 3d_cnn.py           # Training script for 3D CNNs
├── evaluate.py         # Evaluation scripts
├── compare_models.py   # Model comparison scripts
├── results/            # Saved results and metrics
├── requirements.txt    # Dependencies
└── README.md           # Project description
```

## Future Work

- Exploring hybrid models combining 3D CNNs and transformers.
- Extending to multi-modal activity recognition (e.g., audio-video fusion).
- Optimizing models for real-time video analysis.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions and bug reports.

## License

This project is licensed under the [MIT License](LICENSE).

---

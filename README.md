# sign2voice
Web app translating isolated ASL signs into speech, with a comparison of GRU, 1D-CNN and Transformer models on MediaPipe keypoints (WLASL)

Real-time web application that recognizes isolated American Sign Language (ASL)
signs from a webcam and converts them to speech.

## Goals
- Extract hand and upper-body keypoints with MediaPipe
- Compare 3 sequence models (GRU, 1D-CNN, lightweight Transformer)
  on 2 representations (hands only vs. hands + upper body)
- Integrate the best model in a web app with text-to-speech

## Dataset
WLASL (Li et al., 2020), subset of 20-30 common words.
https://github.com/dxli94/WLASL

## Structure
- `src/`: data preparation, models, evaluation
- `notebooks/`: experiments (Colab)
- `app/`: Flask backend and web interface
- `models/`: saved model and scaler
- `results/`: metrics, confusion matrices

## Status
Work in progress (MPDS federated project).

## Limitations
Isolated signs only, small vocabulary, ASL only. This is a communication aid,
not a certified interpreter.

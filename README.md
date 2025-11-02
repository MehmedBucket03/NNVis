# NNVis

# Neural Network Visualizer

Real-time, interactive 3D visualization of neural networks showing neuron activations, weight gradients, and confidence metrics. Backend computations stream to a dynamic React UI to enhance model interpretability.

## Features
- 3D network graph (orbit/pan/zoom, hover/click)
- Live activations, gradients, and confidence metrics
- Step-through training (play/pause/next)
- Model-agnostic PyTorch adapter
- Session recording (JSON frames)
- Light/dark themes

## Quick Start
### Backend
```bash
cd server
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
uvicorn nnviz.main:app --reload --port 8000

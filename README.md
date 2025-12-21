# ROV Object Detection using YOLO

This repository contains a YOLO (You Only Look Once) model trained for object detection in the context of the Singapore Autonomous Underwater Vehicle Challenge (SAUVC). The model is specifically designed to detect underwater objects such as gates, which are common in SAUVC tasks.

## Model Details

- **Model File**: `gate_model.pt`
- **Framework**: PyTorch (assuming based on .pt extension)
- **Purpose**: Detect gates in underwater environments for autonomous navigation and task completion in SAUVC.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/Z1-N/ROV_objectDetection.git
   cd ROV_objectDetection
   ```

2. Install dependencies (assuming Python environment):
   ```
   pip install torch torchvision ultralytics  # or whatever is needed for YOLO
   ```

## Usage

To use the model for inference:

```python
import torch
from ultralytics import YOLO  # assuming Ultralytics YOLO

model = YOLO('gate_model.pt')
results = model('path/to/image.jpg')
results.show()
```

## Training

If you need to retrain the model, refer to the YOLO documentation or provide training scripts.

## Contributing

Feel free to contribute by opening issues or pull requests.

## License

[Add license if applicable]
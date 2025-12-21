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

## Model Metrics

<img src="https://drive.google.com/uc?export=view&id=1VxgLdyZF9TQd-gY9cZL0uHC_uSzWbr-R" alt="Screenshot of the Model metrics" width="800">

## Examples

Here are some examples of the model tested on various competition objects:

<img src="https://drive.google.com/uc?export=view&id=1JLFItT60he9dBL4OjY0Vcbs0cU23_53S" alt="Model Tested on Various Competition Objects" width="600">

<img src="https://drive.google.com/uc?export=view&id=1cq-mnYusr-YcAq_0-jzYlqcQcUvDSPt9" alt="Model Tested on Various Competition Objects" width="600">

## Training

If you need to retrain the model, refer to the YOLO documentation or provide training scripts.

## Contributing

Feel free to contribute by opening issues or pull requests.

## License

[Add license if applicable]
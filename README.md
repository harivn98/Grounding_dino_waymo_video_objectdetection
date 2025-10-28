🦒 Grounding DINO – Text-Based Object Detection

This project uses Grounding DINO to detect objects in images and videos using text prompts like “car”, “person”, or “traffic light”.

🚀 Features

Detect objects using text input

Works on both images and videos

Saves annotated results automatically

Easy to customize detection prompts

⚙️ Setup
# Install dependencies
pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu
pip install supervision transformers addict yapf timm pycocotools opencv-python

# Clone Grounding DINO
git clone https://github.com/IDEA-Research/GroundingDINO.git

# Download model weights
mkdir weights
wget https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth -O weights/groundingdino_swint_ogc.pth

🖼️ Image Detection
detect_and_visualize("path/to/image.jpg", "car . person")

🎥 Video Detection
detect_in_video("path/to/video.mp4", "car . person", frame_interval=30, save_output=True)

📁 Folders
test_images/       # Input images
output_video/      # Annotated videos
GroundingDINO/     # Cloned repo
weights/           # Model weights

🧠 Model Used

Grounding DINO Tiny from IDEA-Research

Zero-shot object detection using text prompts

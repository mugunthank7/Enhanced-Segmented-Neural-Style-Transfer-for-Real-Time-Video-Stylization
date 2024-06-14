# Enhanced Segmented Neural Style Transfer for Video Stylization
## Output
![Alt text](results/background-gif.gif)

## Description
This project focuses on enhancing Neural Style Transfer (NST) for video stylization by incorporating segmentation-based techniques and a temporal loss function. The goal is to apply different artistic styles to distinct regions within video frames while maintaining frame-to-frame coherence. This project leverages the power of deep learning and convolutional neural networks (CNNs) to create visually appealing and artistically consistent videos.

## Project Objectives
1. **Develop a Robust NST Model:** Create a high-quality model capable of performing neural style transfer on both images and videos.
2. **Implement Segmentation-Based Style Transfer:** Apply different styles to specific regions within video frames to enhance creativity and visual appeal.
3. **Incorporate Temporal Loss Function:** Ensure smooth and consistent stylization across video frames to maintain temporal coherence.
4. **Monitor and Evaluate Performance:** Use TensorBoard for tracking training progress and conduct both qualitative and quantitative evaluations to validate the model's performance.

## Features
- **Advanced NST Model:** Utilizes convolutional neural networks (CNNs) to perform high-quality style transfer.
- **Segmentation-Based Style Transfer:** Allows for different artistic styles to be applied to distinct regions within video frames.
- **Temporal Loss Function:** Ensures that the stylization is consistent across consecutive video frames, preventing flickering and other artifacts.
- **Performance Monitoring:** TensorBoard is used to track the training process, visualize metrics, and evaluate the model's performance.
- **Comprehensive Evaluations:** Both qualitative and quantitative methods are used to assess the effectiveness of the style transfer.

## Installation
To get started with the project, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mugunthank7/Enhanced-Segmented-Neural-Style-Transfer-for-Real-Time-Video-Stylization.git
   cd Enhanced-Segmented-Neural-Style-Transfer-for-Real-Time-Video-Stylization
   ```

2. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage
Here is a step-by-step guide to using the project:

1. **Prepare your content and style images:**
   - Collect the images and videos you want to use for content and style transfer.
   
2. **Run the training script:**
   ```bash
   python train.py --content-dir path/to/content --style-dir path/to/style
   ```
   - This script will train the NST model using the provided content and style images.

3. **Generate stylized videos:**
   ```bash
   python stylize_video.py --input-video path/to/video --output-video path/to/output
   ```
   - This script will apply the trained NST model to the input video and save the stylized output.

## Results
Example results showcasing the effectiveness of the enhanced NST model can be found in the `results` folder. These examples demonstrate various stylized videos where different artistic styles have been applied to specific regions within the frames.

## Methodology
### Data Preparation
- **Content Images:** A diverse set of images and videos are used as content sources.
- **Style Images:** Various artistic images representing different styles are used to train the model.

### Model Architecture
- **Base Network:** A pre-trained VGG-19 network is used for feature extraction.
- **Transfer Network:** A feed-forward convolutional network is employed for style transfer.
- **Segmentation Module:** DeepLabV3 or a similar model is used for semantic segmentation to identify different regions within the video frames.
- **Temporal Loss Function:** A custom loss function ensures temporal coherence across frames.

### Training Process
- **Loss Functions:** The training process minimizes a combination of content loss, style loss, and temporal loss to achieve high-quality stylization.
- **Optimization:** The Adam optimizer is used for efficient training.

### Evaluation Metrics
- **Qualitative Evaluation:** Visual inspection of the generated images and videos.
- **Quantitative Evaluation:** Metrics such as Structural Similarity Index (SSIM) and Gram matrix loss are used to assess the model's performance.


## Acknowledgements
- Inspired by the foundational work of Gatys et al., "A Neural Algorithm of Artistic Style" (2015).
- Special thanks to the contributors of TensorBoard for providing a robust tool for performance monitoring.

## Contact
For questions or collaborations, please contact [mugunthankesavan07@gmail.com](mailto:mugunthankesavan07@gmail.com).

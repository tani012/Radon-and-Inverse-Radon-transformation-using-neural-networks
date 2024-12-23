# Efficient Radon Transform and Inverse Reconstruction Using DNNs

This repository implements the use of Convolutional Neural Networks (CNNs) for performing the inverse Radon transform, offering improvements in noise resilience, image quality, and computational efficiency over traditional methods like Filtered Back-Projection (FBP).

## Objectives
- Generate sinograms from synthetic 2D images using the Radon Transform.
- Train a CNN to reconstruct 2D images from sinograms.
- Compare CNN performance with FBP using metrics such as MSE, SSIM, and runtime.
- Explore applications in medical imaging, seismic imaging, and industrial testing.

## Features
- **Noise Handling**: Robust reconstruction from noisy sinograms.
- **Real-Time Performance**: Efficient reconstructions post-training.
- **High Image Quality**: Superior SSIM and MSE scores compared to FBP.

## Getting Started

### Prerequisites and running the project
```bash
pip install -r requirements.txt
python src/generate_data.py
python src/train_model.py
python src/evaluate_model.py
``` 
### Results
- Noise Robustness: CNNs outperform FBP, especially with noisy sinograms.
- Image Quality: Higher SSIM and lower MSE in image reconstruction.
- Efficiency: Real-time inference after training.

### Applications
- Medical Imaging: Enhanced CT scan reconstructions, especially in low-dose imaging.
- Seismic Imaging: Improved reconstruction of incomplete and noisy datasets.
- Non-Destructive Testing: Accurate material inspections using sinogram data.

### Future Work
- Extend the approach to 3D Radon Transform for volumetric imaging.
- Enhance the model's capability for sparse or incomplete data.
- Apply the method to real-world datasets for practical use cases.


# GeoPix Framework for Subsurface Reservoir Characterization

## Overview
The **GeoPix Framework** leverages Generative Adversarial Networks (GANs), specifically the Pix2Pix model, to generate high-resolution property maps such as porosity and permeability from facies images. This model is designed to improve subsurface reservoir characterization by providing more accurate predictions of rock properties.

## Network Architecture

### Generator
- A **U-Net-based architecture** designed to generate property maps (e.g., porosity, permeability) from facies input images.
- The U-Net structure allows for high-quality image-to-image translation by combining convolutional layers with skip connections.

### Discriminator
- A **PatchGAN-based convolutional network** used to evaluate the realism of the generated property maps.
- It operates on image patches to ensure that both global structure and local texture are realistic.

---

### **Architecture of the GeoPix Framework**

![Pix2Pix GAN Architecture](https://raw.githubusercontent.com/ARhaman/GeoPix/main/Figuers/Pix2Pix%20GAN%20rchitecture.png)

---

### **High-level Architecture of the Proposed GeoPix Framework for Subsurface Reservoir Characterization**

![GeoPix Framework](Figuers/Modified_GeoPix_Figure%201.png)


---

## Key Features
- **Data-Driven Modeling**: Utilizes machine learning models to predict rock properties directly from geological facies data.
- **Robust Performance**: The combination of U-Net and PatchGAN improves the generation of high-resolution, geologically plausible property maps.
- **Application in Reservoir Characterization**: The model aids in better understanding subsurface formations, which is critical for hydrocarbon exploration and production.

## Repository Structure

```bash
GeoPix/
├── Figuers/                 # Contains architecture and framework images
├── Examples_of_Results/     # Example output images
├── model/                   # GAN model architecture files
├── data/                    # Training and testing datasets
├── README.md                # Project overview and documentation
└── requirements.txt         # Python dependencies
```


## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/ARhaman/GeoPix.git
   cd GeoPix
2. Install the dependencies:
bash
Copy code
pip install -r requirements.txt
3. Train the model:
bash
Copy code
python train.py --dataset your_dataset --epochs 100
4. Generate predictions:
bash
Copy code
python generate.py --input facies_image.png --output predicted_property.png
Contact
For any questions or collaboration inquiries, please contact:

Abdulrahman Al-Fakih
Ph.D. Researcher | Geophysics
King Fahd University of Petroleum and Minerals (KFUPM)
📞 +966 500916367
📧 g202103050@kfupm.edu.sa



# Galaxy Cluster Dynamic Mass Estimation

![Screenshot (325)](https://github.com/user-attachments/assets/5bcc8ed4-b525-4135-8eec-9efb89ea7fdb)

## Project Description
This project estimates the dynamic mass of galaxy clusters using the virial theorem, based on the positions and redshifts of member galaxies. The implementation includes:

- Velocity dispersion calculation
- Projected size estimation
- Virial mass estimation
- Advanced cosmological corrections
- Bootstrap error analysis
  
## Visualisation

![Screenshot (336)](https://github.com/user-attachments/assets/c7a3f68e-65f8-46f2-a357-20e067956612)


## Formulas Used

### 1. Velocity Dispersion

\[
v = c \cdot \frac{z - z_{\text{cluster}}}{1 + z_{\text{cluster}}}
\]
\[
\sigma_v = \text{Standard Deviation of } v
\]

### 2. Simple Virial Mass Estimation

\[
M = \frac{3 \cdot \sigma_v^2 \cdot R}{G}
\]

### 3. Advanced Mass Estimator

\[
M = \frac{\alpha \cdot \sigma_v^2 \cdot R}{G}
\]
Where \(\alpha = 3\) (structure correction factor)

### 4. Bootstrap Error Estimation

\[
\bar{M} = \text{Mean of Bootstrap Masses}
\]
\[
\Delta M = \text{Standard Deviation of Bootstrap Masses}
\]

    
## Requirements
- Python 3.8+
- Jupyter Lab
- Required packages (see `requirements.txt`)

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/galaxy-cluster-mass.git
   cd galaxy-cluster-mass

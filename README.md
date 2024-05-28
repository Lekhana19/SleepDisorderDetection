# Sleep Disorder Detection Project

## Project Overview
This project focuses on detecting sleep disorders, specifically insomnia, using machine learning and signal processing techniques. It involves the analysis of EEG recordings obtained from both normal and insomnia-affected individuals to classify sleep patterns accurately.

### Key Features
- **Data Source**: EEG recordings from [Physionet](https://physionet.org)
- **Target Audience**: Researchers and healthcare professionals interested in sleep pattern analysis.
- **Technologies Used**: MATLAB for signal processing, Python for machine learning.

## Installation and Usage

### Prerequisites
- MATLAB (for Preprocessing.m and signal processing)
- Python 3.x (for MLalgorithm.py)
- Libraries: numpy, pandas, sklearn

### Steps to Run the Project
1. **Clean the Dataset**:
   - Use the provided scripts to clean the EEG dataset. This step removes noise and irrelevant data.
   
2. **Signal Preprocessing**:
   - Input the cleaned EEG data into `Preprocessing.m`.
   - Perform frequency analysis using discrete Fourier transformation to extract alpha, beta, theta, and delta waves.
   - Apply a cutoff frequency range of 0.5 to 30 Hz.

3. **Feature Extraction**:
   - Extract features such as mean, minimum, maximum, standard deviation, and variance for each wave.
   - Save the extracted features into `output.csv`.

4. **Model Training and Testing**:
   - Load `output.csv` in `MLalgorithm.py`.
   - Use logistic regression to classify the data into normal and insomnia classes.
   - Dataset is split into 70:30 for training and testing, respectively.
   - Training accuracy is expected to be around 100%, with testing accuracy between 60% and 80%.

## Contributing
This project is open for contributions, especially for improving the machine learning model and expanding the dataset. Contributions to enhance the signal processing algorithm are also welcome.

## Team
- Project Mentor: [Your Name]
- Student Contributors:
  -  Lekhana
  -  Naman Bansal
  -  Ajay
  -  Bharath

## Video Link 
https://www.youtube.com/watch?v=o9iA870oCrI&ab_channel=NamanBansal

## Project Website

https://www.leadingindia.ai/internshipproject
https://www.leadingindia.ai/projectdetails/52

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments
- Special thanks to all the contributors from various universities for their dedication and hard work.
- Thanks to [Physionet](https://physionet.org) for providing access to a valuable dataset.

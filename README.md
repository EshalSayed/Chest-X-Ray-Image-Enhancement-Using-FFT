#Chest X-Ray Image Enhancement Using Frequency Domain Analysis
Overview
This project demonstrates frequency-domain enhancement of chest X-ray images using the 2D Fast Fourier Transform (FFT) in MATLAB and Simulink. The objective is to improve structural clarity by separating smooth components from fine anatomical details and applying Gaussian high-pass filtering with FFT-based unsharp masking.
The work connects fundamental Signals and Systems concepts with practical medical image processing applications.

#Project Objectives
Transform a chest X-ray image into the frequency domain using FFT
Analyze magnitude and phase spectra
Design and apply Gaussian low-pass and high-pass filters
Enhance high-frequency anatomical details
Implement both script-based (MATLAB) and block-based (Simulink) solutions

#Methodology
1. Image Preprocessing
Convert image to grayscale if required
Resize to a uniform resolution (512 × 512)
Normalize intensity values for stable processing

2. Frequency Domain Transformation
The image is converted into its frequency representation using the 2D Fast Fourier Transform. The zero-frequency component is shifted to the center for proper spectral visualization.

3. Spectrum Analysis
The magnitude spectrum represents the strength of frequency components
The phase spectrum preserves spatial structure and anatomical positioning
An important observation is that phase information is critical in maintaining the structural integrity of the image.

4. Gaussian Filtering
A Gaussian low-pass filter is designed to model smooth frequency attenuation. The high-pass filter is derived as the complement of the low-pass filter, enabling clean separation between smooth background components and fine structural details.

5. FFT-Based Unsharp Masking
High-frequency components are extracted and added back to the original image using a scaling factor. This enhances edges and anatomical boundaries while maintaining overall image stability.

#Results

The project produces:
Original chest X-ray
Magnitude spectrum
Phase spectrum
Enhanced X-ray using FFT-based unsharp masking
The enhanced image emphasizes rib edges, lung boundaries, and subtle structural transitions while preserving the overall anatomical structure.

#Medical and Technical Relevance

This enhancement is not intended to replace diagnostic imaging. However, it is relevant in the following contexts:
Preprocessing for AI-based medical image analysis
Feature enhancement prior to segmentation
Edge-focused visualization for structural analysis
Educational demonstration of frequency-domain filtering
Simulink Implementation
In addition to MATLAB scripting, the complete enhancement pipeline is modeled in Simulink. This demonstrates:
Block-level signal flow representation
Frequency-domain filtering using system blocks
Real-time visualization of processed output
The dual implementation strengthens the engineering depth of the project by combining theoretical DSP concepts with system-level modeling.


#Skills Demonstrated

Digital Signal Processing
Frequency-domain image analysis
MATLAB programming
Simulink system modeling
Gaussian filter design
Practical application of Signals and Systems concepts

#Conclusion

This project demonstrates how classical DSP techniques such as FFT, Gaussian filtering, and unsharp masking can be applied to medical image enhancement. It highlights the importance of frequency-domain analysis and reinforces the practical value of foundational signal processing concepts.

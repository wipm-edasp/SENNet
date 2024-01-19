SENNet: Spectrum-Edited Neural Network for 1H NMR Spectral Signals Separation
Introduction

Nuclear magnetic resonance (NMR)-based untargeted metabolomics studies rely on specific NMR pulse sequences, such as 1D nuclear Overhauser effect spectroscopy (NOESY), 1D Carr-Purcell-Meiboom-Gill (CPMG) spectroscopy, and 1D diffusion-edited spectroscopy, to detect distinct NMR signatures from small molecules and lipoproteins in plasma or serum samples. However, conducting NMR experiments on batch samples can be time-consuming.

To address this issue, we have developed the Spectrum-Edited Neural Network (SENNet). This model enables efficient and accurate separation of spectral signals from macromolecules and small molecules, providing an end-to-end mapping from the entire metabolome NMR spectrum to the macromolecular and small molecule NMR spectra.
Methodology

We applied the SENNet method to post-process 1D NMR NOESY-presat spectra obtained from 120 plasma samples and 463 serum samples. The method successfully separated signals from both large and small molecules in these spectra. Comparison with experimental spectra from 1D CPMG and 1D diffusion-edited experiments demonstrated the effective extraction of all small molecule signals. Principal component analysis (PCA) performed on the large and small molecule signals showed comparable statistical information to analyses conducted using experimental data, indicating the reliability and efficiency of the SENNet method for signal extraction.
Usage

The trained model can be applied to commonly used NOESY-presat spectra collected from a 600 MHz NMR spectrometer in metabolomics. By utilizing the SENNet method, researchers can achieve more accurate separation of molecular signals in plasma and serum, enhancing the quality and efficiency of their metabolomics studies.
Benefits and Potential

The Filter-Unet method offers several advantages:

    Time Efficiency: This high-throughput untargeted NMR post-processing method reduces the time spent on conducting NMR experiments on batch samples, improving research efficiency.
    Accurate Signal Separation: The method effectively separates signals from both large and small molecules within 1D NOESY-presat spectra, providing reliable and comprehensive spectral information.
    Metabolic Biomarker Discovery: By facilitating the extraction of small molecule signals, the Filter-Unet method holds significant potential for the discovery of metabolic biomarkers in metabolomics research.
    Versatility: While the method has been primarily validated using plasma and serum samples, it can potentially be applied to other sample types, expanding its range of applications.
    Integration Potential: The SENNet method can be integrated with other analytical methods to enhance the characterization of metabolomic profiles and facilitate further insights into metabolic processes.

Future Directions

Future developments and improvements for the Filter-Unet method include:

    Evaluation on Diverse Sample Types: Further testing is required to assess the performance of the method on a wider variety of sample types, including tissues and other biological fluids.
    Integration with Other Analytical Methods: Exploring the integration of the Filter-Unet method with complementary analytical techniques, such as mass spectrometry, could provide more comprehensive metabolomic analysis.
    Enhanced User-Friendly Implementation: Efforts will be made to develop user-friendly software tools or libraries that enable easy application of the Filter-Unet method for NMR-based metabolomics studies.

License

This project is licensed under the MIT License.
Conclusion

The SENNet method offers an efficient solution for the separation of spectral signals in NMR-based metabolomics. By accurately extracting small molecule signals from 1D NOESY-presat spectra, it enhances research efficiency and facilitates the discovery of metabolic biomarkers. The method has been successfully applied to plasma and serum samples, demonstrating its reliability and potential for high-throughput data post-processing. We anticipate that the Filter-Unet method will contribute to advancing metabolomics research and inspire further exploration in this field.

Please note that the SENNet method is an ongoing research project, and we welcome collaboration and feedback from the scientific community to improve and expand its applications. If you have any questions, comments or suggestions about the program, please contact us at the following: xiaoxj007@outlook.com

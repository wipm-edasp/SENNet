# SENNet

This repository contains the software implementation of the Spectral Editing Neural Network (SENNet) model, which can distinguish signals of small and macromolecules based on the linewidth at half-height of spectral peaks, and generate the spectra of small and macromolecules simultaneous from blood 1H NOESY-presat spectra, to shorten the experimental time of NMR based metabolomics study. The detailed description can be found in the paper titled "[Using neural networks to obtain NMR spectra of both small and macromolecules from blood samples in a single experiment](https://doi.org/10.1038/s42004-024-01251-x))".

Installation

This is a Python program that runs in the form of an IPython Notebook (.ipynb) file. Before running it, make sure you have the following tools and dependencies installed:

    torch - 1.7.1
    numpy - 1.22.4
    matplotlib - 3.5.1

File Structure

    README.md: This file provides an overview of the project and instructions for usage
    MTBLS242_noesypr1d_10.npy: Contains numpy.array format of the first 10 noesypr1d spectra of the MTBLS242 dataset
    models_baseline_0711.py:Basic model
    model_snnet_trained.pkl:The trained snnet model
    run_model.ipynb:This is an interactive file consisting of a series of cells. It allows users to run the model cell by cell in this IPython Notebook file
    Run_model_600MHz_ML242.ipynb：Example of Processing MTBLS242 (600 MHz) Data
    Run_model_700MHz.ipynb：Example of processing 700 MHz serum plasma data
    MTBLS374_SENNet_output_mean.npy：Contains numpy.array format of the MTBLS374 output by SENNet
    MTBLS2387_PE003_cpmg.npy: Contains numpy.array format of MTBLS2387 PE003 cpmgpr1d (plsama)
    MTBLS2387_PE003_noesy.npy: Contains numpy.array format of MTBLS2387 PE003 noesypr1d (plsama)
    MTBLS2387_SE003_cpmg.npy: Contains numpy.array format of MTBLS2387 SE003 cpmgpr1d (serum)
    MTBLS2387_SE003_noesy.npy: Contains numpy.array format of MTBLS2387 SE003 noesypr1d (serum)
    plasma_noesypr1d.txt: The choose plsama noesypr1d as base data 
    read_120plasma_forpaper.ipynb: read 120 plasma data for paper
    read_ML242_forpaper.ipynb: read ML242 data for paper
    read_ML374.ipynb: read ML242 data for paper
    
    LICENSE: This file contains the project's license information.

Introduction

SENNet is a neural network-based approach designed to separate spectral signals in untargeted metabolomics studies that rely on nuclear magnetic resonance (NMR). By utilizing specific NMR pulse sequences, such as 1D NOESY, 1D CPMG, and 1D diffusion-edited spectroscopy, SENNet can accurately detect distinct NMR signatures from small molecules and lipoproteins in plasma or serum samples.

Usage

The trained SENNet model is applicable to NOESY-presat spectra commonly collected from a 600/700 MHz NMR spectrometer in metabolomics research. With SENNet, researchers can achieve more accurate separation of molecular signals in plasma and serum, enhancing the quality and efficiency of their metabolomics studies.

Benefits and Potential

SENNet offers several advantages:
- Time Efficiency: This high-throughput method reduces the time spent on conducting NMR experiments, improving research efficiency.
- Accurate Signal Separation: SENNet effectively separates signals from both large and small molecules within 1D NOESY-presat spectra, providing reliable and comprehensive spectral information.
- Metabolic Biomarker Discovery: By facilitating the extraction of small molecule signals, SENNet holds significant potential for discovering metabolic biomarkers in metabolomics research.
- Versatility: Although primarily validated with plasma and serum samples, SENNet can potentially be applied to other sample types, expanding its range of applications.
- Integration Potential: SENNet can be integrated with other analytical methods to enhance the characterization of metabolomic profiles and gain further insights into metabolic processes.

Future Directions

Future developments and improvements for SENNet include:
- Evaluation on Diverse Sample Types: Further testing is needed to assess the performance of SENNet on a wider variety of sample types, including tissues and other biological fluids.
- Integration with Other Analytical Methods: Exploring the integration of SENNet with complementary analytical techniques, such as mass spectrometry, could provide more comprehensive metabolomic analysis.
- Enhanced User-Friendly Implementation: Efforts will be made to develop user-friendly software tools or libraries that enable easy application of SENNet for NMR-based metabolomics studies.

License

This project is licensed under the MIT License.

Conclusion

SENNet offers an efficient solution for the separation of spectral signals in NMR-based metabolomics. By accurately extracting small molecule signals from 1D NOESY-presat spectra, it enhances research efficiency and facilitates the discovery of metabolic biomarkers. The method has been successfully applied to plasma and serum samples, demonstrating its reliability and potential for high-throughput data post-processing. We welcome collaboration and feedback from the scientific community to improve and expand the applications of SENNet, as it continues to evolve as an ongoing research project. If you have any questions, comments, or suggestions, please contact us at xiaoxj007@outlook.com.

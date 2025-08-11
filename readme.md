# OCR-Beatrice_Moxon_diary1885

## Description

This project is a OCR system for the Beatrice Moxon diary 1885. It uses the TrOCR model to perform OCR on the images. It also uses the LLMs to improve the accuracy of the OCR.

## Usage

1. Create a anaconda environment with the required packages.
> `conda env create -f environment.yml`
2. Activate the environment.
3. Run TrOCR.ipynb to test the generate reference text for the images.
4. Run gemini.ipynb to get the finetuned text for the images.

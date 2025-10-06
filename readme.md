# Optical Character Recognition (OCR) of the Beatrice Moxon Diary 1885

This project is an Optical Character Recognition (OCR) system for the diary of Beatrice Moxon from 1885. It uses the TrOCR model for OCR and is enhanced with Large Language Models (LLMs) to improve accuracy. This tool is designed to digitize and analyze historical handwritten documents.

The detail of the project process can be found in the project page: **[Optical Character Recognition (OCR) of the Beatrice Moxon Diary](https://tasrif-khondaker.github.io/OCR-Beatrice_Moxon_diary1885/)**

## Description

The primary goal of this project is to develop an accurate, efficient pipeline for transcribing historical handwritten documents using TrOCR for OCR and LLM-based post-processing. The workflow emphasizes image preprocessing, model inference, LLM-assisted correction, and systematic evaluation to improve overall transcription quality. This repository documents the end-to-end process with notebooks and configuration files so others can reproduce and adapt the pipeline to their own archival scans.

![Fig: Architecture of the proposed OCR pipeline](https://github.com/tasrif-khondaker/OCR-Beatrice_Moxon_diary1885/blob/Page/src/Architecture.svg?raw=true "Architecture of the proposed OCR pipeline")


## Dataset

The original scanned images (Pages of Beatrice Moxon's 1885 diary) and any processed dataset created for this project are not publicly available due to privacy/copyright/donor restrictions. To reproduce the pipeline, run the included notebooks (TrOCR.ipynb and gemini.ipynb) on your own scans or sample data. If you require access for legitimate research purposes, please contact the maintainer via the project page linked above.

We have shared some sample images in the `_data.ipynb` notebook to help you get started.

## Requirements

The following packages are required to run the code:

- Python 3.8+
- Anaconda
- Jupyter Notebook
- PyTorch
- Transformers
- PIL
- OpenCV
- LangChain
- OpenAI / Gemini / other LLM API access
- Other dependencies listed in environment.yml

## Getting Started

Follow these steps to set up and run the project on your local machine.

### Prerequisites

  * Anaconda or Miniconda installed on your system.

### Installation

1.  **Clone the repository:**

    ```sh
    git clone https://github.com/tasrif-khondaker/OCR-Beatrice_Moxon_diary1885.git
    cd OCR-Beatrice_Moxon_diary1885
    ```

2.  **Create and activate the Conda environment:**

    ```sh
    conda env create -f environment.yml
    conda activate ocr_beatrice
    ```

### Usage

1.  **Generate Reference Text:**
    Run the `TrOCR.ipynb` notebook to process the diary images and generate the initial OCR text.

2.  **Fine-Tune with LLM:**
    Run the `gemini.ipynb` notebook to apply the LLM for enhancing the accuracy of the transcribed text.

    > Note: Currently, the notebook is set up to use Gemini API. 
    > You can modify it to use other LLMs as needed.
    > Make sure to set your API keys in the notebook.

## Repository Structure

```bash
OCR-Beatrice_Moxon_diary1885/
├── Data/
│   └── GroundTruth/
├── Results/
│   └── Gemini/
├── api_key/
│   └── api.json
├── ocr_output_ref/
├── .gitignore
├── TrOCR.ipynb
├── _data.ipynb
├── claude.ipynb
├── environment.yml
├── gemini.ipynb
├── prompt.json
└── readme.md
```

## Contributing

Contributions are welcome\! If you have any suggestions or find any issues, please feel free to open an issue or submit a pull request.

## Links

  * **Project Page:** [https://tasrif-khondaker.github.io/OCR-Beatrice\_Moxon\_diary1885/](https://tasrif-khondaker.github.io/OCR-Beatrice_Moxon_diary1885/)
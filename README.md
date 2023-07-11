# Receipt Scraper

Receipt Scraper is a Python script that extracts details from images of receipts and stores the information in a CSV file. It utilizes the Mindee API for optical character recognition (OCR) and document parsing. The project consists of two notebooks: `test_ground.ipynb` and `main.ipynb`.

## Prerequisites

Before running the notebooks, make sure you have the following:

- Python 3.6 or above installed
- Mindee API key. You can obtain the API key by signing up on the [Mindee website](https://www.mindee.com/)

## Installation

Clone the repository or download the notebook files.

## Usage

### Individual Receipt Scraper

The `test_ground.ipynb` notebook allows you to extract information from a single receipt image. To use it:

1. Open the `test_ground.ipynb` notebook in Jupyter Notebook or JupyterLab.

2. Obtain your Mindee API key and update the `api_key` variable in the notebook with your API key.

   ```python
   # Init a new client
   mindee_client = Client(api_key="your_api_key")
3. Follow the instructions in the notebook to load an individual receipt image, process it, and view the extracted information.

### Multiple Receipts Scraper 

The main.ipynb notebook enables you to process multiple receipts stored in a folder. To use it:

1. Open the main.ipynb notebook in Jupyter Notebook or JupyterLab.

2. Obtain your Mindee API key and update the api_key variable in the notebook with your API key.

   ```python
   # Init a new client
   mindee_client = Client(api_key="your_api_key")
3. Create a folder and place the receipt images you want to process inside it.
/Receipts
    ├── receipt1.jpg
    ├── receipt2.jpg
    ├── receipt3.jpg
    └── ...
4. Update the folder_path variable in the notebook with the path to the folder containing the receipt images.
  
    # Folder path containing the receipts
    folder_path = "path/to/your/folder"
5. Follow the instructions in the notebook to process the multiple receipts, extract the information, and view the combined results in a CSV file named receipts.csv.


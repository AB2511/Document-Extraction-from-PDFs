# Document-Extraction-from-PDFs
# Document Extraction from PDFs  

A Python-based project to extract and structure text from PDF documents. This program reads a user-provided PDF file, processes its content, and organizes it into a structured JSON format for better usability and analysis.

## Features  
- **PDF Text Extraction**: Reads and extracts all text content from PDF files using the PyMuPDF library.  
- **Data Categorization**:  
  - **Headers**: General text, titles, or paragraph content.  
  - **List Items**: Structured/tabular data, such as items resembling table content.  
- **JSON Output**: Converts the extracted and categorized content into a clean, human-readable JSON format.  
- **Cloud Integration**: Built and tested on Google Colab, with integration for Google Drive for seamless file handling and sharing.  

## Technologies Used  
- **Python**  
- **PyMuPDF (fitz)**  
- **JSON**  
- **Google Colab**  

## How to Use  
1. Clone this repository:  
   ```bash  
   git clone https://github.com/AB2511/Document-Extraction-from-PDFs.git  
   cd Document-Extraction-from-PDFs  
   ```  
2. Open the provided `.ipynb` notebook in Google Colab or any Python IDE.  

3. Provide the path to the PDF file you want to extract text from. If using Google Colab, upload your PDF file to your Google Drive and use its path.  

4. Run the notebook. The extracted text will be categorized and saved as a JSON file.  

5. Download the generated JSON file or access it directly from your Google Drive (if using Colab).  

## Example  
### Input:  
A PDF file containing the following content:  
```
Title: Project Report  
Table 1: Key Statistics  
```

### Output (JSON):  
```json  
{
  "headers": [
    "Title: Project Report"
  ],
  "list_items": [
    "Table 1: Key Statistics"
  ]
}
```

## Installation  
Install the required Python libraries:  
```bash  
pip install pymupdf
```

## File Structure  
- `Document-Extraction.ipynb`: Main notebook containing the code for PDF extraction and JSON generation.  
- `README.md`: Project description and usage instructions.  


Happy coding! 🚀

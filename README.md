# PDF-Entity-Recognition
PDF Entity Recognition is a Python script that utilizes the SpaCy library to extract named entities from PDF files. It performs named entity recognition on the text extracted from the PDF and provides options to save the recognized entities in different formats such as HTML, JSON, or CSV.

Installation
Clone the repository or download the script file.

Install the required dependencies using the following command:

Copy code
pip install spacy PyPDF2
Additionally, you may need to install the SpaCy English language model by running the command:

Copy code
python -m spacy download en_core_web_lg
Usage
Ensure that you have the PDF file(s) you want to process.

Run the script using the following command:

Copy code
python pdf_entity_recognition.py
The script will prompt you to select the input PDF file or directory using a file dialog.

Choose the input file or directory, and the script will process the PDF file(s) and extract the named entities.

The recognized entities will be displayed in the console, and depending on your configuration, they will be saved in the specified output format (HTML, JSON, or CSV). The output files will be named "entities_output" for single file processing and "<filename>_entities_output" for batch processing.

Additional Options
Output Format: By default, the recognized entities are saved in HTML format. You can modify the output_format variable in the script to change the output format to JSON or CSV.

Batch Processing: If you provide a directory as the input, the script will process all the PDF files in that directory. The recognized entities will be saved for each individual file.

Error Handling and Logging
The script includes error handling and logging to record any errors or exceptions that occur during file processing or entity recognition. Error messages will be displayed in the console, and detailed information will be logged in the error.log file

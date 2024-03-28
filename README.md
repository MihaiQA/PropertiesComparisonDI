# PropertiesComparisonDI
Comparison of Giata xml`s and properties.tsv file.
# Property Data Comparison Tool

## Description

This tool automates the comparison of property ratings from two data sources: TSV files and XML files. It processes property ratings from a specified TSV file, compares these against ratings found in XML files within a specified directory, and generates a detailed comparison report in a PDF document. This solution is ideal for ensuring data consistency across property information maintained in different formats.

## Features

- Reads property ratings from TSV files.
- Parses and compares property ratings from XML files.
- Outputs comparison results to the console and a PDF report.

## Setup and Installation

**Requirements:**
- Python 3.x
- `lxml` library for XML parsing.
- `reportlab` library for generating PDF reports.

**Steps:**

1. **Clone the repository:**
   ```bash
   git clone https://your-repository-url.git
   cd your-project-directory

    Install required libraries:
    Ensure you have Python and pip installed on your machine. Install the required libraries using:

    bash

    pip install lxml reportlab

Project Structure

    main_script.py: The primary script that orchestrates reading from TSV, comparing XML files, and generating the PDF report.
    requirements.txt: Contains a list of project dependencies for easy installation via pip.
    properties.tsv: Sample TSV file containing property ratings.
    /xml_properties: Directory containing sample XML files with property data.

Usage

    Prepare your TSV file (properties.tsv) with property ratings.
    Place your XML files within the /xml_properties directory.

Run the script:

bash

python main_script.py

This will generate a PDF report named comparison_results.pdf, detailing the comparison between the TSV data and each of the XML files processed.
Python Script Breakdown

The script is composed of several functions:

    increase_csv_field_size_limit(): Increases the CSV field size limit to accommodate large fields.
    read_from_tsv_file(tsv_file_path): Reads properties and their ratings from a TSV file.
    read_and_compare_xml_file(xml_file_path, tsv_properties, pdf): Parses an XML file, compares it against the TSV data, and appends findings to a PDF.
    compare_xml_files_in_directory(directory_path, tsv_properties, pdf): Iterates through XML files in a specified directory for comparison.
    main(): Orchestrates the workflow of reading TSV data, comparing XML files, and generating the PDF report.

Ensure to adjust file paths and names as necessary to match your project setup.
Contributing

Contributions are welcome! If you have suggestions for improvements or bug fixes, please fork the repository and submit a pull request.
License

For additional questions or feedback, feel free to open an issue in the repository.

less


Remember to replace placeholders like `https://your-repository-url.git`, `your-project-dire

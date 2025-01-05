# AUTOMATED-REPORT-GENERATION

**Name**: ADIL SHAIKH

**Company**: CODETECH IT SOLUTIONS

**ID**: CT08DJS

**Domain**: Python Programming

**Duration**: 12th December to 12th January

**Mentor**: Neela Santhosh Kumar

# OUTPUT OF THIS PROJECT

# PROJECT:AUTOMATE REPORT GENERATION
![OUTPUT](https://github.com/user-attachments/assets/12767853-d9eb-411c-bb05-354592e6a7e4)



This code is a complete Python script that reads data from a CSV file, analyzes the data, and generates a PDF report summarizing the analysis.
Here’s an overview of each part of the code:

# 1. Importing Libraries:

The script imports the csv module for reading CSV files and the FPDF class from the fpdf library for creating PDF documents.

# 2. Reading Data from CSV:

The function read_data_from_csv(file_path) is defined to read data from a specified CSV file.
It initializes an empty list called data.
It opens the CSV file in read mode and uses csv.DictReader to read the rows as dictionaries.
For each row, it extracts the 'Name' and 'Value' fields, converting 'Value' to a float, and appends a dictionary containing these fields to the data list.
The function returns the list of dictionaries.

# 3. Analyzing Data:

The function analyze_data(data) takes the list of dictionaries as input.
It extracts the 'Value' from each dictionary into a list called values.
It calculates the average, maximum, and minimum of the values.
The function returns these three statistics.

# 4. Generating PDF Report:

The function generate_pdf_report(data, average, maximum, minimum, output_file) creates a PDF report.
It initializes a new PDF document and adds a page.
It sets the font and adds a title to the report.
It includes a line break and then adds the analysis results (average, maximum, and minimum values) to the PDF.
Another line break is added before creating a table to display the original data.
The function creates a table with headers ('Name' and 'Value') and populates it with the data from the input list.
Finally, it saves the PDF to the specified output file.

# 5. Main Function:

The main() function serves as the entry point of the script.
It defines the input CSV file name (data.csv) and the output PDF file name (report.pdf).
It calls the read_data_from_csv function to read the data from the CSV file.
It then calls the analyze_data function to compute the average, maximum, and minimum values.
Finally, it calls the generate_pdf_report function to create the PDF report and prints a message indicating that the report has been generated.

# 6. Execution:

The script checks if it is being run as the main program and calls the main() function to execute the workflow.

Overall, this code provides a straightforward way to read numerical data from a CSV file, perform basic statistical analysis, and generate a well-formatted PDF report containing the results and the original data.
It demonstrates the use of file handling, data manipulation, and PDF generation in Python.

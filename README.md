# Resume Scanner

Resume Scanner is a Python script that compares a resume against a job description to calculate a matching score and identify common keywords. It helps in automating the initial resume screening process by providing insights into the relevance of a resume to a specific job posting.

## Features

- Extracts text from PDF and DOCX resume files
- Downloads job descriptions from a given URL
- Identifies keywords from the job requirements or qualifications section
- Calculates a matching score between the resume and job description
- Displays the matching score and common keywords found in both the resume and job description

####### Requirements

- Python 3.x
- spaCy
- PyPDF2
- python-docx
- requests
- beautifulsoup4

## Installation

1. Clone the repository:
2. Navigate to the project directory:
3. Create a virtual environment (optional but recommended):
    ```
    python -m venv venv
    ```


5. Activate the virtual environment:
- For macOS and Linux:
  ```
  source venv/bin/activate
  ```
- For Windows:
  ```
  venv\Scripts\activate
  ```

5. Install the required libraries:
   ```
   pip install -r requirements.txt
   ```
7. Download the spaCy English model:
   ```
   python -m spacy download en_core_web_lg
   ```

######## Usage

1. Run the script:
  python resumeScanner.py

2. Enter the URL of the job posting when prompted.

3. Enter the path to the resume file (PDF or DOCX) when prompted.

4. The script will process the resume and job description, and display the matching score and common keywords.

## Customization

- If the script fails to find the requirements or qualifications section on the job posting webpage, you may need to adjust the `download_job_description()` function in the script to match the specific HTML structure of the website you are scraping.

- The script currently supports PDF and DOCX resume formats. If you need to support other file formats, you can add the corresponding extraction functions in the script.

## Modifications

- Modified the repository to create a HTML plugin from the source python code, which can be used to scan for keywords in .pdf or .docx files uploaded onto a web interface.
    - Also updated the Python code in 'resumeScanner.py' by making it more effecient, less resource-intensive, and by fixing 2 bugs.     

- Added the "Frontend (HTML)" file to create a folder named templates and within it, create a file named index.html for the frontend interface.

- Added the "Flask Set-Up" file to to set up the  Flask application. Install Flask and the required packages using pip.

- Added the "Backend (Flask App)" file for the backend logic.

- Added the "App Execution" file to run the Flask application.

- Final step is to navigate to 'http://127.0.0.1:5000/' in your browser.

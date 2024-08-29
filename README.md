Text Analysis Module

This project performs analysis of text documents, including statistical calculation, frequency terms, n-gram generation, concordance and preservation of unique words. It provides a simple interface for processing several directories with text files.

Installation I uploaded my files on GitHub to avoid issues with opening all files. To open it, you need to follow next steps:

1. Clone the repository

Clone the repository to your local machine:

git clone https://github.com/undmargo/corpus-linguistics-with-python-final-project.git

2. Change to the project directory:

cd corpus-linguistics-with-python-final-project

3. Install dependencies

In my zip.file or GitHub page, you'll see the requirements.txt which is a text file that lists all the dependencies (libraries and Python packages) that the project needs to run. It easily installs all the necessary packages in your development environment or on a server.

What is its purpose? When someone else (lecturers or me with another computer) wants to install and run the project, having requirements.txt allows automatically installing all the necessary packages with a single command.


# This command creates the file
​
pip freeze > requirements.txt
​
Note: you may need to restart the kernel to use updated packages.
This command helps to install all dependencies using the command, once requirements.txt is created

pip install -r requirements.txt

4. Usage

To run the example script that analyzes a directory of text files, use the following command:

python run_analysis.py /path/to/text/files

IMPORTANT! You need to replace /path/to/text/files with the path to the directory containing your text files. The script will generate analyses based on the text files in the specified directory.

5. Features

Here is the list of implemented features with explanations:

Load Documents: loads text documents from a specified directory. Compute Statistics: calculates basic statistics such as the number of lines and tokens in every document. Term Frequency: computes term frequency for every document and globally. Type-Token Ratio: calculates the type-token ratio for every document and globally. N-grams: generates unigrams, bigrams, and trigrams for every document and globally. Concordance: generates concordance for a written word in texts. Collocations: finds collocations (bigrams or trigrams) in texts. Unique Words: generates and saves unique words from the text.

6. Dependencies

The reason why this project was created on the uni server with JupyterLab is that it was impossible to upload nltk library on my Macbook for further work. So, after looking into the list of requirements we see that nltk (and matplotlib, which is also an another important library for creating graphs) are present.

This project requires the following Python libraries:

nltk matplotlib

These dependencies were mentioned in the requirements.txt file. You can install them using pip.

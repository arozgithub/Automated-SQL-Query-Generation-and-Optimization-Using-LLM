`Automated SQL Query Generation and Optimization using OpenAI`


This project demonstrates how to automate the generation and optimization of SQL queries using OpenAI's GPT models. The application reads a user's query request, generates an appropriate SQL query, executes it, and provides optimization suggestions.

`Features`

`_SQL Query Generation:` Automatically generates SQL queries based on user input.
`SQL Query Optimization: `Optimizes generated SQL queries to improve performance.

`API Integration:` Leverages OpenAI API for AI-based query generation and optimization._

`Execution and Results:` Runs the generated SQL queries and returns results.
Prerequisites
Before you begin, ensure you have met the following requirements:


OpenAI API Key
Required Python libraries (see below)
Libraries Required
Install the necessary libraries using pip:


pip install openai prettytable python-dotenv pdfplumber
Setup
`Clone the repository:`
git clone https://github.com/yourusername/automated-sql-query-generation.git

cd automated-sql-query-generation
Install dependencies:

pip install -r requirements.txt
`Create an .env file or api.txt to store your OpenAI API key.`

Run the notebook or script to generate and optimize SQL queries based on user input.

`API Setup`
The OpenAI API key is required for this project. Place your API key in the api.txt file, which will be read in the script:


with open("api.txt") as f:
    openai.api_key = f.read().strip()
Usage
The main function reads SQL query requests from an input file (input.txt), generates the corresponding SQL query, optimizes it, and executes it.

`Here’s the key function breakdown:`

generate_sql(): Generates the SQL query based on the question provided.
optimize_sql(): Provides an optimized version of the generated SQL query.
execute_sql(): Executes the query and fetches the results.

`Example`

Provide questions in the input.txt file, and the script will process them:

What is the average salary of employees in the HR department?

The system will:

**Generate the SQL query.**
Optimize it.
Execute the query and return the result.

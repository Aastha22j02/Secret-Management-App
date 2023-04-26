# README

## Introduction
This code is a simple Streamlit application that reads secret variables stored in Streamlit Secrets and environment variables, and prints their values. The purpose of this code is to demonstrate how to access secrets in Streamlit, and how to compare them with their corresponding environment variables.

## Usage
To use this code, follow these steps:
1. Clone the repository
2. Create a file named `.env` in the root directory of the project, and set the values for the environment variables `db_username` and `db_password`. Example:
   ```
   db_username=my_db_username
   db_password=my_db_password
   ```
3. Create a file named `.streamlit/secrets.toml` in the root directory of the project, and set the values for the secrets `db_username` and `db_password`. Example:
   ```
   [db_username]
   value = "my_db_username"

   [db_password]
   value = "my_db_password"

   [my_cool_secrets]
   things_i_like = "streamlit, python, machine learning"
   ```
4. Run the code using the command `streamlit run app.py`.
5. The application should launch in your browser, displaying the values of the secrets and environment variables.

## Dependencies
This code requires the following dependencies:
- Streamlit
- Python-dotenv

You can install them using pip by running the following command:
```
pip install streamlit python-dotenv
```
# Testmo - Python - Selenium - Playwright 

Testmo provides its own CLI client, which I strongly recommend using. I want to avoid using JavaScritp at all, so I decide to create my own Python client for Testmo. I used the OpenAPI provided by Testmo: https://docs.testmo.com/api/schema/openapi

This is an unofficial Python CLI version of Testmo OpenAPI.

## Put this files to the root of your test project
If you have already installed dependecy from requirements.txt then ommit step 1 - setup your env

## 1. Setup your env 
1. Create venv into .vevn folder
2. Install deps from requirements.txt file

## 2. Setup your Testmo API 
1.  Visit Testmo [API Authentication](https://docs.testmo.com/api/introduction/api-authentication) 
2. Add your url and token to .env 

## 3. Run the tests
1. Execute `pytest . -s -v` command staying in the root of the framework
2. To form a report execute `pytest . --junitxml=results/test-results.xml -s -v`  command

## 4. Send your automation jUnit raport to the endpoint of Testmo 

run testmo

`python testmo_cli.py source name`

source: str
name: str

eg. `python testmo_cli.py VSC Tests `



 PS: Example report in results/test-results.xml

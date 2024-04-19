




<h1 align="center">⭐ API Testing using Pytest Framework </h1>

<p align="left">  
# Introduction -- There are 3 microservices that are running when the backend is up.

🔷 Signup service -- Service for user to create his account. After account is created a token is returned. This token is needed to access other two services. If one forgets his token, he can renew his token.

🔷 Quote service -- Quotation service. This generates random quotes. One will need to provide token provided by the signup service

🔷 Weather service -- Weather service. This generates random weather. One will need to provide token provided by the signup service

</p>

## To Get Started 🚀🚀🚀

### ➡ Pre-requisites

- Download and install Python:

  🟢 [Install Python](https://www.python.org/downloads/ "Install Python")

- Download and install any Text Editor like Visual Code/Sublime/Brackets

  🟢 [Install Visual Studio Code](https://code.visualstudio.com/download "Install Visual Studio Code")

### ➡ Setup

- Clone the repository into a folder
- Go to Project root directory and install Dependency: `pip install -r requirements.txt`🚀
- All the dependencies from requirements.txt will be installed.

## ➡ How to run services 🚀🚀

All the services are containerised. Hence you will need docker to be installed already on your system.

If you do not have it installed on your machine, you can download it from [here](https://www.docker.com/products/docker-desktop).

Once docker is running, follow these steps --

From the root of the folder run following command in terminal
`docker-compose up -d`.

## ➡Run Test 😀

1. Open Terminal
2. Go to project location
3. Enter `pytest -v` and hit enter key 🚀
4. To capture stdout Enter
   `pytest -sv --capture=sys` and hit enter key

### ➡ Generate HTML Report using pytest-html

1. Open Terminal
2. Go to project location
3. Enter `pytest --html=report.html`' and enter key 🚀

Must watch 😀 

https://github.com/VishakhaThakur2021/pytest-api-automation-vscode/assets/86808541/2e87be70-4563-439d-8fa8-c74cc61a89ab



## ➡ HTML Report 🚀🚀

![HTML Test Report](./screenshot_results/html-image.png)

<img width="956" alt="html-image" src="https://github.com/VishakhaThakur2021/pytest-api-automation-vscode/assets/86808541/623bac8c-1c96-47de-a92e-0fe2f10e70b3">

In the above screenshot get_user test is failing here,
expected output is not equal to actual output 🤔



### ➡ Pre-requisites before generating allure report 🤔

1. Open Terminal , Go to project location and write `pip install allure-pytest`

2. Go through the guidelines https://allurereport.org/docs/pytest/
3. Install https://scoop.sh/ command-line tool for windows

## ➡ Generate Allure Report using pytest-allure

1. Open Terminal
2. Go to project location
3. Enter `python -m pytest --alluredir allure-results` and then `allure serve allure-results` 🚀 hit enter

Must watch 😀 

https://github.com/VishakhaThakur2021/pytest-api-automation-vscode/assets/86808541/c8c85c71-03ec-4500-bd01-0b536d35d4e3





## Allure Report 🚀🚀





<img width="935" alt="allure-image" src="https://github.com/VishakhaThakur2021/pytest-api-automation-vscode/assets/86808541/b841e91a-56c0-4d3d-a7ef-6c4899a03f36">


![HTML Test Report](./screenshot_results/allure-image.png)

In the above screenshot get_user test is failing here,
expected output is not equal to actual output 🤔







## ➡ How to connect sqlite3 in vscode 🚀🚀

1. Go to extensions in vscode
2. Search for SQlite and install
3. Go to View > Command Palette > SQlite open database > Choose database from file
4. Click on run ▶ tab on table
5. User can inspect newly created record in database
6. Download sqlite using [DB Browser for SQLite](https://sqlitebrowser.org/).

<img width="921" alt="sqlite-image" src="https://github.com/VishakhaThakur2021/pytest-api-automation-vscode/assets/86808541/42e77d6e-4160-4afd-8cfb-6b2fdb019c16">

![HTML Test Report](./screenshot_results/sqlite-image.png)

👉 Note : Services runnning on ports number 8081 (docker-compose.yml and nginx_config.conf)

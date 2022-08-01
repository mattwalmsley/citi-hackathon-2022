# citi-hackathon-2022
Team C set-up guide. Edit as appropriate.

## Download Python and Git
- [Python](https://www.python.org/downloads/)
- [Git](https://github.com/git-guides/install-git)

## Clone the GitHub repo
Navigate to a local folder and run:

    git clone git@github.com:mattwalmsley/citi-hackathon-2022.git

## Set-Up Python Virtual Environment

Create virtual environment with venv module (run this in citi-hackathon-2022 directory)

<br>
Linux:

    python3 -m venv .venv

<br>
Windows/Mac (probably):

    python -m venv .venv

- [Using the command line](https://docs.python.org/3/using/cmdline)
- [venv](https://docs.python.org/3/library/venv.html)

<br>
Activate virtual environment:

    source .venv/bin/activate

<br>
Setting for settings.json in .vscode

    {
    "python.defaultInterpreterPath": "${workspaceFolder}/.venv/bin/python3",
    "python.envFile": "${workspaceFolder}/.venv"
    }

<br>
Install required packages for venv from file:

    pip install -r requirements.txt

<br>
Write/updates required packages for venv to requirements file:

    pip freeze > requirements.txt

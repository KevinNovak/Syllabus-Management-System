## Setup for Windows

### 1. Installing Python (includes Pip)
- Go to https://www.python.org/downloads/
- Download and install the newest version of Python 3
- While installing, make sure to check box for adding python to the system PATH

### 2. Installing VirtualEnv with Pip
- Open up command prompt, and type in the following command:
> pip install virtualenv
- Once virtualenv is installed, in command prompt navigate to your user folder (where documents, pictures, etc. are)
- Type in the following command
> virtualenv virtualenv

### 3. Installing Project Requirements with Pip
- In command prompt, navigate to the project folder (where requirements.txt is)
- Type in the following command
> pip install -r requirements.txt

### 4. Running Server
- While in the project folder, type the following command
> python run.py
- The server is now running, and viewable at the printed address (likely https://127.0.0.1:5000/)

## Centos 7 Setup

### 1. Install all dependencies

    yum install python-devel python-virtualenv libffi-devel gcc openssl-devel

### 2. Setup a virtual environment
    virtualenv /path/to/venv
	source /path/to/venv/bin/activate
	pip install -U pip

### 3. Install requirements
    pip install -r requirements.txt

### 4. Run the server
	python run.py

## Debian Jessie Setup

### 1. Install all dependencies

    apt install python3-dev python3-venv libffi-dev gcc libssl-dev

### 2. Setup a virtual environment
    python3 -m venv /path/to/venv
	source /path/to/venv/bin/activate

### 3. Install requirements
    pip install -r requirements.txt

### 4. Run the server
	python run.py

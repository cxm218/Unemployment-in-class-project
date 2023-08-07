# Unemployment-in-class-project

## Setup

Obtain an [AlphaVantage API Key](https://www.alphavantage.co/support/#api-key). A normal key should be fine, but alternatively you can use one of the prof's "premium" keys. Then create a faile called '.env' and place it inside (like following)

```sh
# this is the ".env" file (in the root directory of the repo)

ALPHAVANTAGE_API_KEY="____________"

Create a virtual environment:

```sh
conda create -n unemployment-env python=3.10
```

```sh
conda activate unemployment-env
```

Install third-party packages:

```sh
pip install -r requirements.txt
```

## Usage

Run the report:

```sh
python app/unemployment.py

python -m app.unemployment

```
Run the web app using the following code: 

# Mac OS
FLASK_APP=web_app flask run

# Windows OS:
# ... if `export` doesn't work for you, try `set` instead
# ... or try a ".env" file approach
export FLASK_APP=web_app
flask run
## Testing

Run tests:

```sh
pytest
```
## [Deployment Guide](/DEPLOYING.md)
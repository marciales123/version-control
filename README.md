# my-first-app-fall-2024

## Setup

Create a virtual environment (first time only):

```sh
conda create -n reports-env-2024 python=3.10
```

Activate the environment (whenever you come back to this project):

```sh
conda activate reports-env-2024
```

Install packages:

```sh
pip install -r requirements.txt
```

[Obtain an API Key](https://www.alphavantage.co/support/#api-key) from AlphaVantage.

TODO inclue instructions here for signing up for email sending platform. Obtain mailgun API ey, and set the key an sender address as env vars. 
Create a ".env" file and add contents like the following (using your own AlphaVantage API Key):

```sh
# this is the ".env" file:
ALPHAVANTAGE_API_KEY="..."

#optionally:

MAILGUN_SENDER_ADDRESS = userdata.get("____________") # "example@georgetown.edu"
MAILGUN_DOMAIN = userdata.get("____________") # "sandbox-xyz.mailgun.org"
MAILGUN_API_KEY = userdata.get("____________")
```


## Usage

Run the example script:

```sh
python app/my_script.py
```

Run the unemployment report:

```sh
#ALPHAVANTAGE_API_KEY="..." python app/unemployment.py

python app/unemployment.py
```

Run the stocks report:

```sh
python app/stocks.py
```

Run the example email sending file:

``` sh
python app/email_service.py
```

Run the RPS game: 
```sh
python app/rps.py 
```

##Testing

Run tests: 

```sh
pytest
```


# streamlit-heroku-template

a simple template for deploying a Streamlit app on Heroku

## Requirements

- Python 3.9
- Poetry [Documentation](https://python-poetry.org/docs/)

## How-to

### Install packages

```{bash}
poetry install
```

### Run app

```{bash}
poetry run streamlit run src/app.py --server.runOnSave true
```

### Format code

```{bash}
poetry run yapf src/* -i -p
```

### Deploy to Heroku

Export requirements

```{bash}
poetry export -f requirements.txt --without-hashes --output requirements.txt
```

Go through [Heroku: Deploying with Git](https://devcenter.heroku.com/articles/git)

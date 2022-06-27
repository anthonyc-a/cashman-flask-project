## Flask RESTful API

### Running the API

To run this application, you will need Python 3+ and [Pipenv](https://pipenv.readthedocs.io/en/latest/) installed locally. If you do, you can issue the following commands:

```bash
# from the flask-restful-apis directory
pipenv install
./bootstrap.sh 
```

Then you can issue requests to your API. For example, with `curl`, you can issue requests like:

```bash
# inserting a new income
curl -X POST -H "Content-Type: application/json" -d '{
    "amount": 300.0,
    "description": "loan payment"
}' http://localhost:5000/incomes

# listing all incomes
curl http://localhost:5000/incomes
```

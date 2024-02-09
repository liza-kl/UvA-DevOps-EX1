# UvA-DevOps-EX1
UvA DevOps Assignment 1 

## Notes 
- How to start the API

1. Generate the Python Code
2. In the `requirements.txt` change the following 

```
connexion[swagger-ui] == 2.14.0
flask == 2.2.3 
tinydb == 4.8.0
```

3. Run `python3 setup.py install `
4. cd `./swagger_server `
5. python3 `__main__.py`
6. Open the project `README.md` there is the correct URL to access the UI

- For the Docker had to adjust the `workflows/main.yml`, in order to make it running
with the current folder structure. 
# Flask app

## Start up

1.  ```
    mkdir <flask app>
    ```
2.  ```
    poetry init -n
    ```
3.  ```
    poetry add flask
    ```
4.  ```
    poetry export -f requirements.txt -o requirements.txt
    ```
5.  insert into app.py
    ```py
    from flask import Flask
    app = Flask(__name__)


    @app.route('/')
    def hello():
        return "Hello World!"

    if __name__ == '__main__':
        app.run()
    ```
6.  ```
    python app.py
    ```
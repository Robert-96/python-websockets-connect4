# python-websockets-connect4

An WebSocket server for a Connect Four game.

## Install

To get started, install the required dependencies using pip:

```
pip install -r requirements.txt
```

## Development Setup

### Server

After installing the dependencies, run the following command to start the server:

```
python server/app.py
```

During development, use `watchmedo` to automatically restart the server upon code changes. First, install the required tool:

```
pip install -r requirements-dev.txt
```

Then, execute:

```
watchmedo auto-restart --pattern "*.py" --recursive --signal SIGTERM python server/app.py
```

### UI

Start an HTTP server:

```
cd ui
python -m http.server
```

Open http://localhost:8000/ in a web browser.

## License

This project is licensed under the [MIT License](LICENSE).

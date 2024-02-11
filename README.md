# Twitter Trends API

This is a simple FastAPI application that interacts with Twitter's "Trends" API and saves the trending topics in a MongoDB database.

## Prerequisites

- Python 3.12
- Docker
- Twitter Developer Account

## Setup

1. Clone the repository:

```sh
git clone <repository-url>
cd <repository-directory>
```

2. Create a `secrets.py` file in the `src` directory with your Twitter API keys:

```python
CONSUMER_KEY = 'your-consumer-key'
CONSUMER_SECRET = 'your-consumer-secret'
ACCESS_TOKEN = 'your-access-token'
ACCESS_TOKEN_SECRET = 'your-access-token-secret'
```



Replace

 `'your-consumer-key'`, `'your-consumer-secret'`, `'your-access-token'`, and `'your-access-token-secret'` with your actual keys and tokens.

3. Build the Docker image:

```sh
docker build -t twitter-trends-api .
```

4. Run the Docker container:

```sh
docker run -p 8000:8000 twitter-trends-api
```

The application will be available at `http://localhost:8000`.

## Endpoints

- `GET /trends`: Returns a list of trending topics from the Twitter API.

## Running Tests

To be implemented.

## Contributing

To be implemented.

## License

To be implemented.

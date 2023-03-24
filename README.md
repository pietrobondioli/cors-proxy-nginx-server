# Cors Proxy Nginx Server

This is a simple nginx proxy server that allows you to proxy requests to a remote server and add CORS headers to the response. This is useful if you want to proxy requests to a remote server that does not allow CORS or if you want to proxy requests to a remote server that does not allow requests from a specific domain.

It was created to save time when developing a frontend application that needs to make requests to a remote server that does not allow CORS.

## Usage

### ENV Variables

| Variable | Description |
|----------|-------------|
| `REMOTE_HOST` | The remote server to proxy requests to |
| `EXPOSED_PORT` | The port to expose the proxy server on |

*Important*: Before running the container, make sure that the variables is correctly set, it should be put on `.env` file at the root of the project (check `.env.sample`).

### Running the container

```bash
docker-compose up -d
```

## License

MIT License

Copyright (c) 2022 Pietro Bondioli

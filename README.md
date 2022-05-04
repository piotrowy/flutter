# Flutter

Flutter docker image to automate builds in CI/CD pipelines.

## Usage
```dockerfile
FROM piotrowy/flutter:1.0 AS webBuilder

# Copy files to container and build
COPY app .
RUN flutter build web --dart-define=apiAddress=${API_ADDRESS}
```
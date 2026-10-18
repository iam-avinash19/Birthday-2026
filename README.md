# Hema's Birthday Website (Docker)

## Run with Docker
    docker build -t hema-birthday .
    docker run -d --name hema-birthday -p 8080:8080 hema-birthday

Open http://localhost:8080

## Or with Docker Compose
    docker compose up -d --build

## Stop / remove
    docker compose down      # compose
    docker rm -f hema-birthday   # plain docker

## Notes
- Container runs nginx as a non-root user on port 8080.
- Fonts load from Google Fonts, so the viewer needs internet.
- To change the page, edit index.html and rebuild the image.

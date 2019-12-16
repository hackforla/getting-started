## Developing via Docker

Docker is the recommended approach to quickly getting started with local development.

There are two pre-requisites: Docker and Docker Compose.
The recommended installation method is [Docker Desktop][dockerdesktop] for Windows 10 64-bit,
Mac, and Linux users. Users of unsupported operating systems may check out [Docker Toolbox][dockertoolbox] instead.

More on using Docker and the concepts of containerization:

* [Get started with Docker][docker]
* [Get started with Docker Compose][dockercompose]

*Ensure you run the `docker` commands below from a shell inside the local directory containing your clone of this repository.*

### Build and serve the website locally

This command starts a jekyll server locally. The server watches for changes to
the source files and rebuilds and refreshes the site automatically in your browser.

```bash
docker-compose up
```

Now browse to http://localhost:4000

### Tear down

To stop and completely remove the jekyll server (i.e. the running Docker container):

*(do this anytime Docker or jekyll configuration or other repository settings change)*

```bash
docker-compose down
```

To stop the server, but not destroy it (often sufficient for day-to-day work):

```bash
docker-compose stop
```

Bring the same server back up later with:

```bash
docker-compose up
```

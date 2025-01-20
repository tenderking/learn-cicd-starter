![code coverage badge](https://github.com/tenderking/learn-cicd-starter/actions/workflows/ci.yml/badge.svg)
# learn-cicd (Notely)

Welcome to the "Notely" application for the "Learn CICD" course on [Boot.dev](https://boot.dev). The main purpose is to apply dev principles and show case a CI/CD pipeline using github actions.
It includes:
- a ci pipeline for linting, tests and security checks
- a cd pipeline for db migrations and a deployment to gcp.
- sqlc for data modeling and code generation for db
- dockerfile for turning app to  a docker container which will be deplyoed on gcp

## Local Development

Make sure you're on Go version 1.23+.

Create a `.env` file in the root of the project with the following contents:

```bash
PORT="8080"
```

Run the server:

```bash
go build -o notely && ./notely
```

*This starts the server in non-database mode.* It will serve a simple webpage at `http://localhost:8080`.


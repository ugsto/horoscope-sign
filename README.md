# Sign

This application is a simple horoscope application. For reference on the
frontend, consult the appllication
[here](https://github.com/ugsto/horoscope-sign-frontend), as for the backend,
please, take a look [here](https://github.com/ugsto/horoscope-sign-backend).

## How to run

To run the whole application, you can use the docker-compose file provided in
the root of the project. To do so, you need to have docker and docker-compose
installed. Then, you can run the following command:

```bash
docker-compose up
```

This will start the frontend and the backend. The frontend will be available
at `https://localhost:8443` and the backend at `http://localhost:3000`.

## Configuration

Configurations are done through environment variables, they can be configured
through the `.env` in each submodule and through the `docker-compose.yaml` file.

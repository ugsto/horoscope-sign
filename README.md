# Sign

This application is a simple sign horoscope generator with a frontend and a
backend. The frontend is written in React and uses the backend to generate
horoscopes. The backend is written in TypeScript using Express to serve the API.

## Configuration

The application is configured using environment variables that may be
configured in each frontend and backend. Please, refer to the README files in
each directory for more information.

Each variable in the specific part of the application is available in the
docker-compose configuration, as they are passed to the containers as
environment variables. So, if you want to change the configuration, you can do
it in the docker-compose file.

| Variable    | Description                      | Default                                    | Scope    |
| ----------- | -------------------------------- | ------------------------------------------ | -------- |
| GPT_URL     | The URL of the GPT API           | https://api.openai.com/v1/chat/completions | Backend  |
| GPT_API_KEY | The API key for the GPT API      |                                            | Backend  |
| GPT_MODEL   | The model to use for the GPT API | gpt-3.5-turbo                              | Backend  |
| HOST        | The host to bind to              | 0.0.0.0                                    | Backend  |
| PORT        | The port to bind to              | 3000                                       | Backend  |
| API_URL     | The URL of the backend API       | http://localhost:3000/api/v1/sign          | Frontend |

## How to use

To start the application from docker-compose, run:

```bash
docker-compose up
```

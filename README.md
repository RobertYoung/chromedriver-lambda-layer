# ChromeDriver Serverless Lambda Layer

## Setup

Unzip `lib/extract-me-here.zip`

## Deploy

```sh
npm run deploy:test
npm run deploy:prod
```

## Usage

serverless.yml

```yml
functions:
  run-test:
    handler: handler.runTest
    layers:
      - arn:aws:lambda:eu-west-1:xxxxxx:layer:chromedriver:1
```
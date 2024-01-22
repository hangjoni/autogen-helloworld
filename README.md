## About

A multi-agents system to chat with database.

Example output for query `"how much did user 101 spend"`
[example output](./imgs/example_output.png)

## How to run

- Create .env file with similar structure as .env.sample
- Run in terminal:
  `poetry run start --prompt "how much did user 101 spend"`

## TODO:

- It's working now but unstable with the parsing of text. Let's use a json library or get the api to return json next

## Changelog

- v1: working infrastructure for querying about database
- v2: add multi agent support

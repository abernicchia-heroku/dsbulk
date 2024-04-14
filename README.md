# dsbulk
Run DataStax Bulk Loader on Heroku - it can be used to inspect Cassandra clusters

## Deploying to Heroku

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## How to run it

```sh
$ heroku run console -a <your heroku app name>

# once your one-off dyno is running
~ $ cd dsbulk-1.11.0/bin
~ $ ./dsbulk count -h <host> -u <user name> -p <user password> -k <keyspace> -t <table> 
~ $ ./dsbulk unload -h <host> -u <user name> -p <user password> -k <keyspace> -t <table>
~ $ ./dsbulk load -h <host> -u <user name> -p <user password> -k <keyspace> -t <table> 
```

## Documentation

For more information about using DataStax Bulk Loader, see these articles:

- [DataStax Bulk Loader](https://downloads.datastax.com/#bulk-loader)
- [DataStax Bulk GitHub repository](https://github.com/datastax/dsbulk)
- [DataStax Bulk Loader CLI options](https://docs.datastax.com/en/dsbulk/docs/reference/reference-index.html)
- [dsbulk load examples](https://docs.datastax.com/en/dsbulk/docs/reference/load.html#dsbulk-load-examples)
- [dsbulk unload examples](https://docs.datastax.com/en/dsbulk/docs/reference/unload.html#dsbulk-unload-examples)
- [dsbulk count examples](https://docs.datastax.com/en/dsbulk/docs/reference/count-examples.html#dsbulk-count-example)
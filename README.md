# Local Jupyter Environment

my local Jupyter environment for local tests

## FAQ

* Why? for testing stuff when is not possible (or not desirable) to run on Google Colab.

## Run it yourself

first clone the repository, then you'll need to create a `.env` file with the following parameters:

```shell
JUPYTER_TOKEN=YOUR_ACCESS_TOKEN
APP_PORT=10000 # The port you want to run
```

Note: you can also leave the token parameter as `--NotebookApp.token=''` to enter without using authentication.

Now start the container and have fun:

```shell
docker compose up -d --build
```

Note: create your projects inside `work` directory, otherwise it will not appear in your machine volume folder.

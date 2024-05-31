# void
A repository with no working changes

<hr/>

## RenovateBot is not creating PR's for poetry files related to OSV security updates

*How to run this configuration* ?

```shell
$ docker run -it --rm \
    --env LOG_LEVEL=debug \
    --env RENOVATE_CONFIG_FILE=/tmp/renovate/renovate.json \
    --env RENOVATE_PLATFORM=github \
    --env RENOVATE_TOKEN=*** \
    -v path/to/config:/tmp/renovate/renovate.json \
    renovate/renovate:37.320.1
```

*What was expected* ?

I expected the script to create PRs for the vulnerable package `idna@2.8`, which has a fixed version `idna@3.7`. 
However, Renovate Bot is failing to create PRs for OSV vulnerabilities in Poetry files, although it successfully
resolves vulnerabilities and creates PRs for `requirements.txt` files.

*Output logs*

```shell

```
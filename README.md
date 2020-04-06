# docker-aws-cli

![build latest](https://github.com/craighurley/docker-aws-cli/workflows/build%20latest/badge.svg)
![build 1](https://github.com/craighurley/docker-aws-cli/workflows/build%1/badge.svg)

Run `aws-cli` in a container.

## Running

```sh
# Set the AWS_PROFILE environment variable and pass it to the container
AWS_PROFILE=example
docker run --rm -it -v $HOME/.aws:/root/.aws:ro -v $PWD:/workdir:ro -e AWS_PROFILE craighurley/aws-cli
```

Optional: create an alias for the container:

```sh
alias aws-cli='docker run --rm -it -v $HOME/.aws:/root/.aws:ro -v $PWD:/workdir:ro -e AWS_PROFILE craighurley/aws-cli'
```

## Links

- <https://docs.aws.amazon.com/cli/index.html>

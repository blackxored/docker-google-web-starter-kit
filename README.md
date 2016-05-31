# google-web-starter-kit

[![](https://badge.imagelayers.io/blackxored/google-web-starter-kit:latest.svg)](https://imagelayers.io/?images=blackxored/google-web-starter-kit:latest)

Google's [Web Starter Kit](http://developers.google.com/web/starter-kit) Docker-aided workflow for multi-device websites


## Usage

### Bootstrapping a new project

```shell
$ mkdir myproject && cd myproject
$ docker run --rm -p 3000:3000 -p 3001:3001 -v "$(pwd)":/usr/src/app blackxored/google-web-starter-kit
```

This will also start the included HTTP server.

### Running the server

```shell
$ docker run --rm -p 3000:3000 -p 3001:3001 -v "$(pwd)":/usr/src/app blackxored/google-web-starter-kit
```

### Running WSK commands

This image defaults to the `gulp serve` command to run a development server.
See the [documentation](https://github.com/google/web-starter-kit/blob/master/docs/commands.md) for a list of available commands.
Notice the `gulp` keyword is not required for convenience and `build` is the equivalent command to running `gulp` without arguments,
since we've switched the default.

Examples:

```shell
$ docker run --rm -v "$(pwd)":/usr/src/app blackxored/google-web-starter-kit build
```

```shell
$ docker run --rm -p 3000:3000 -p 3001:3001 -v "$(pwd)":/usr/src/app blackxored-google-web-starter-kit serve:dist
```

## License

For license information on the software included in this image, see
[Web Starter Kit LICENSE](https://github.com/google/web-starter-kit/blob/master/LICENSE).

## Supported Docker versions

This image is officially supported on Docker version 1.11.1.

Please see the [Docker installation documentation](https://docs.docker.com/installation/) for details on how to upgrade
your Docker daemon.

## User Feedback

### Issues

If you have any problems with or questions about this image, please make
contact through a [GitHub issue](https://github.com/blackxored/docker-google-web-starter-kit/issues).

## Contributing

You are invited to contribute new features, fixes, or updates, large or small;
we are always thrilled to receive pull requests, and do our best to process
them as fast as we can.

Before you start to code, we recommend discussing your plans through a GitHub
issue, especially for more ambitious contributions. This gives other
contributors a chance to point you in the right direction, give you feedback on
your design, and help you find out if someone else is working on the same
thing.


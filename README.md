# owenthewizard/runit

A basic runit environment to be used as a base for multi-service containers.

Patched to terminate correctly in Docker.

## Quick Start

```Dockerfile
FROM owenthewizard/runit:2.12-r1_alpine

RUN apk --no-cache add example_daemon

COPY example-daemon-runit /etc/service/
# optional
COPY your-runit-1-2-3 /etc/runit/
```

## Contributing

Pull requests are always welcome.

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be licensed under the terms of the [CC0 1.0 Universal](LICENSE.md).

## Versioning

This project is versioned according to the `runit` version, optionally with the release appended.
For example, `2.1.2-r3` would be the third release of this project based on `runit` 2.1.2.

Changes are documented in the [Changelog](CHANGELOG.md).

## Authors

`runit` - cross-platform Unix init scheme with service supervision by [Gerrit Pape](mailto:pape@smarden.org).

See [the list of contributors](https://github.com/owenthewizard/runit/contributors).

## License

See [LICENSE.md](LICENSE.md) for license details of code belonging to this project.

See [LICENSE-RUNIT.txt](LICENSE-RUNIT.md) for license details of the `runit` project by [Gerrit Pape](mailto:pape@smarden.org)

## Acknowledgments

- [Gerrit Pape](http://smarden.org/pape) for [runit](http://smarden.org/runit/) - cross-platform Unix init scheme with service supervision. 

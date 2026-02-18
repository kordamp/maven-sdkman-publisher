# Maven SDKman Publisher

Automated publishing of Apache Maven releases to [SDKman](https://sdkman.io/).

## Background

Publishing new Apache Maven releases to SDKman currently depends on a single person manually triggering an API call.
This repository provides a GitHub Actions workflow to make the process more resilient, accessible, and auditable.

See [Discussion #156](https://github.com/support-and-care/maven-support-and-care/discussions/156) for the full proposal.

## Features

- **Workflow dispatch**: Manually trigger publishing with version input
- **PR-based publishing**: Update a version file via PR, merge triggers the publish
- **Version verification**: Checks the version exists on Maven Central before publishing
- **Default version control**: Choose whether a release should be set as SDKman default
- Uses the official [sdkman-release-action](https://github.com/sdkman/sdkman-release-action) and [sdkman-default-action](https://github.com/sdkman/sdkman-default-action)

## Usage

_TODO: Usage instructions will be added once the workflows are implemented._

## License

This project is licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

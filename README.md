# Orchard

Orchard is a native (swift) application to manage containers on macOS using the new [Containerization framework](https://github.com/apple/containerization).

It has been based on years of experience with Docker Desktop, but dedicated to the new containerization option.

The ambition of the project is to allow it easy for developers to switch from Docker Desktop to Containers. Orchard gives you a desktop experience that complements the `container ...` command-line interface.

![container overview screen](assets/overview.png)

## Highlight of Containerization

- Made by Apple: Native support, incredible performance and the engineering resources to make it work.
- Sub second startup times
- Kernel isolation by design
- Easier networking - no more port mapping (every container gets its own IP address), networks out of the box

## Requirements

> `container` relies on the new features and enhancements present in macOS 26. Additionally, you need to install a specific version of container - [follow the instructions here](https://github.com/apple/container?tab=readme-ov-file#install-or-upgrade) if you have not already upgraded.

https://github.com/apple/container?tab=readme-ov-file#requirements

## Versioning

Since the container project is releasing frequently with breaking changes, starting from `v1.6.0` the releases of this project will track the compatibility with container and mirror them with the difference being `v1` - this is because previous releases used that and it will be impossible to automtically update existing instances.

So, `v1.6.0` supports container `0.6.0` - all changes with that container version will be incremented so the next update will be `v1.6.1`.

When container `0.7.0` is released, the first support will be added in `v1.7.0` of this app.

## Installation

You can build from source or download a prebuilt package.

### Prebuilt

1. Download the latest release from [GitHub Releases](https://github.com/andrew-waters/orchard/releases)
2. Open the `.dmg` file and drag Orchard to your Applications folder
3. Launch Orchard - you may need to go to **System Settings > Privacy & Security** and click "Open Anyway" to allow the app to run

### Build from Source

```bash
git clone https://github.com/andrew-waters/orchard.git
cd orchard
open Orchard.xcodeproj
```

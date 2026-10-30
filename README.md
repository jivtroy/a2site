# Create or delete an Apache2 site

Interactive scripts for creating and deleting virtual hosts in Apache 2. These scripts allow you to create and edit configuration files, add entries to the `/etc/hosts` file, and set up site directories — all via a single CLI command.

### Contents

1. [Compatibility](#compatibility)
2. [Installation](#installation)
   1. [Snap](#snap)
   2. [Build](#build)
3. [Usage](#usage)
   1. [Site creation](#site-creation)
   2. [Site removing](#site-removing)
4. [Removing](#removing)
5. [Author](#author)
6. [License](#license)

## Compatibility

Name | Version
------- | -------
Ubuntu | >= 22.04
Apache | >= 2

## Installation

### Snap

```bash
sudo snap install a2site --classic
```

### Build

Alternative build from source code.

```bash
sudo snap install snapcraft --classic
snapcraft pack --destructive-mode
sudo snap install ./a2site_version_amd64.snap --classic --dangerous
```

## Usage

### Site creation

```bash
sudo a2mksite
```

### Site removing

```bash
sudo a2rmsite
```

## Removing

To completely remove the package run the command:

```bash
sudo snap remove a2site
```

## Author

* [Dev](https://dev.to/jivtroy)
* [Medium](https://medium.com/@jivtroy)
* [YouTube](https://www.youtube.com/@jivtroy)

## License

This project is licensed under the **MIT License** - see the `LICENSE` file for details.
# Apache 2 site

Apache 2 HTTP Server site creation and removing tools using command line.

### Contents

1. [Compatibility](#compatibility)
2. [Installation](#installation)
   1. [Snap](#snap)
3. [Usage](#usage)
   1. [Site creation](#site-creation)
   2. [Site removing](#site-removing)
4. [Removing](#removing)
5. [Author](#author)
6. [License](#license)

## Compatibility

Name | Version
------- | -------
Ubuntu | >= 16.04
Apache | >= 2

## Installation

### Snap

```bash
```

## Usage

### Site creation

```bash
sudo a2mksite mydomain mysite.conf ~/myfolder 127.0.0.1
```

This command will create:

* Virtual host `/etc/apache2/sites-available/mysite.conf` with url http://mydomain.
* Folder `~/myfolder`.
* Record in `/etc/hosts` - mydomain   127.0.0.1.

#### Short command

```bash
sudo a2mksite mydomain
```

This command will create:

* Virtual host `/etc/apache2/sites-available/mydomain.conf` with url http://mydomain.
* Folder in current directory with name mydomain.
* Record in `/etc/hosts` - mydomain   127.0.0.1.
* Restart web server.

### Site removing

```bash
sudo a2rmsite mydomain mysite.conf ~/myfolder 127.0.0.1
```

#### Short command

```bash
sudo a2rmsite mydomain
```

## Removing

To completely remove the package run the command:

```bash
sudo apt remove --purge a2site
```

## Author

* [Dev](https://dev.to/jivtroy)
* [Medium](https://medium.com/@jivtroy)
* [YouTube](https://www.youtube.com/@jivtroy)

## License

This project is licensed under the **MIT License** - see the `LICENSE` file for details.
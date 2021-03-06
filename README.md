*Please :star: this repo if you find it useful*

# Notice

This repository are not meant to be used by a user, but as a "blueprint" that developers
can build upon, to make more awesome stuff.

HAVE FUN! 😎

## Why?

This is simple, by having... #todo

## What?

This repository contains multiple files, here is a overview:

File | Purpose
-- | --
`...` | #todo

## How?

* …or create a new repository on the command line:
    ```bash
    # Initialize your new origin repository
    git init
    git remote add origin https://github.com/YOUR_NEW_REPOSITORY

    # Apply blueprint repository
    git remote add blueprint https://github.com/Limych/py-blueprint.git
    git fetch blueprint dev
    git reset --hard blueprint/dev
    git branch -M dev

    # Push changes to origin repository
    git push -u origin main
    ```

* …or apply blueprint to an existing repository from the command line:
    ```bash
    # Apply blueprint repository
    git remote add blueprint https://github.com/Limych/py-blueprint.git
    git fetch blueprint dev
    git merge blueprint/dev --allow-unrelated-histories

    # Push changes to origin repository
    git push -u origin main
    ```

After these steps, your repository will developing on a own branch. But in parallel there will be this blueprint repository, new changes in which you can always apply with a couple of simple commands:
```bash
./bin/update
git merge blueprint/dev
```

***
README content if this was a published component:
***

*Please :star: this repo if you find it useful*

# Blueprint Client

[![PyPI version][pypi-shield]][pypi]
[![PyPI Python version][pypi-pyversion]][pypi]
[![Maintained][Maintained]](#)

[![Project Maintenance][maintainer-shield]][maintainer]

_Blueprint sample client library._

## Installation

```bash
python3 -m pip install -U blueprint_client
```

## Usage example

```python
from blueprint_client.client import Client

username = "user"
password = "pass"

client = Client(username, password)

data = client.get_data()

client.change_something(True)
```

## Contributions are welcome!

This is an active open-source project. We are always open to people who want to
use the code or contribute to it.

We have set up a separate document containing our [contribution guidelines](CONTRIBUTING.md).

Thank you for being involved! :heart_eyes:

## Authors & contributors

The original setup of this library is by [Andrey "Limych" Khrolenok](https://github.com/Limych).

For a full list of all authors and contributors, check [the contributor's page][contributors].

## License

MIT License

See separate [license file](LICENSE.md) for full text.

[contributors]: https://github.com/Limych/py-blueprint/graphs/contributors
[license]: https://github.com/Limych/ha-blueprint/blob/main/LICENSE.md
[license-shield]: https://img.shields.io/pypi/l/blueprint_client.svg?style=popout
[maintained]: https://img.shields.io/maintenance/yes/2021.svg?style=popout
[maintainer]: https://github.com/Limych
[maintainer-shield]: https://img.shields.io/badge/maintainer-Andrey%20Khrolenok%20%40Limych-blue.svg?style=popout
[pypi]: https://pypi.org/project/blueprint_client/
[pypi-pyversion]: https://img.shields.io/pypi/pyversions/blueprint_client.svg?style=popout
[pypi-shield]: https://img.shields.io/pypi/v/blueprint_client.svg?style=popout

# package_reviewer

A tool to review packages for Sublime Text
(and its package manager Package Control).
Supports passing local file paths
or URLs to GitHub repositories.

This README focuses on installation and usage of the tool.
For how to *resolve* failures or warnings
reported by the tool,
[refer to the wiki][wiki].


## Installation

Requires **Python 3.4** or higher.

```bash
$ git clone https://github.com/packagecontrol/package_reviewer.git
$ cd package_reviewer
$ virtualenv venv
$ source venv/bin/activate  # Windows: .\venv\Scripts\activate.bat
$ pip install -r requirements.txt
```


## Usage

```
$ python -m package_reviewer --help
usage: python -m package_reviewer [-h] [--repo-only] [--verbose] [--debug]
                                  path_or_URL [path_or_URL ...]

Check a Sublime Text package for common errors.

positional arguments:
  path_or_URL    URL to the repository or path to the package to be checked.

optional arguments:
  -h, --help     show this help message and exit
  --repo-only    Do not check the package itself and only its repository.
  --verbose, -v  Increase verbosity.
  --debug        Enter pdb on excpetions. Implies --verbose.
```

For how to resolve failures or warnings
reported by the tool,
refer to the [wiki][].


[wiki]: https://github.com/packagecontrol/package_reviewer/wiki
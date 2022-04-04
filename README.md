# Reddit /r/place 2022 headless bot

This headless Python bot will automatically login to reddit, obtain access 
tokens (and refreshes them when they expire), obtain orders from the C&C server
and automatically place pixels at the desired locations.

## Requirements

- Python >= 3.8
- NumPy
- Matplotlib
- Rich
- aiohttp
- tomli

## Installation & updating to a new version

First you need to install Python to run the script.

### Windows

Go install Python 3.10 on this link: https://www.python.org/downloads/windows/

Create a folder (wherever you want) and right-click "Open in Command Prompt":

Paste the following command in the the command prompt:

```bash
python -m pip install --force git+https://github.com/PlaceNordic/rPlace2022.git
```

### Mac

Go install python 3.10 via the app-store.

Paste the following command in your terminal:

```bash
python -m pip install --force git+https://github.com/PlaceNordic/rPlace2022.git
```

### Linux

Go install python 3.10 via your package manager.

Paste the following command in your terminal:

```bash
pip install --force git+https://github.com/PlaceNordic/rPlace2022.git
```

If you have an older version of Python already installed (or if it gives you errors), try using pip3 instead.

## Usage

### Specifying users in a config file

Besides specifying the username and password combinations on the command line, it's also possible to specify them
in a TOML config file. TOML is an INI-like file format, see the `config-example.toml` for an example.

To specify the path to the config file, add the `--from-config` flag (shorthand: `-c`):

```bash
PlaceNL --from-config config.toml
```

# Doomsday

The [Doomsday Algorithm](https://rudy.ca/doomsday.html) gives the day of
the week for any date (and you can do it in your head).

## Usage

```sh
$ doomsday --help
Usage: doomsday [OPTIONS] [YEAR]

positional arguments:
  YEAR                  year to find doomsday for

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show version information and exit
  -c, --copyright       show copying policy and exit
  -r, --reminder        show doomsday algorithm reminder and exit
  -f FORMAT, --format FORMAT
                        date format (default ‘%A’: full weekday name)
```

## Examples

```sh
$ doomsday              # current year (2015)
Saturday
$ doomsday -f '%F'      # use a custom format
2015-02-28
$ doomsday 1968         # 1968, a leap year
Thursday
```

## Requirements

Should run on Python 3 and newer iterations of Python 2 without
any modifications.

## Installation

Just drop it somewhere in your `$PATH`, e.g., `~/.local/bin/` or
`/usr/local/bin/` — that's all. However, if your Python interpreter is
not installed as `/usr/bin/python` you will have to change the shebang
line to e.g.

```sh
#!/usr/bin/env python
```

Don't worry, be happy :smile:

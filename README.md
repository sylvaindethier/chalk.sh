# :crayon::computer: chalk.sh [![Build Status](https://travis-ci.org/sylvaindethier/chalk.sh.svg?branch=master)](https://travis-ci.org/sylvaindethier/chalk.sh)

> <quote>Terminal string styling done right</quote> -- with bash


## Install

Get a local copy by either:
- Add as submodule:
  ```bash
    $ git submodule add https://github.com/sylvaindethier/chalk.sh.git
  ```
- Clone:
  ```bash
    $ git clone https://github.com/sylvaindethier/chalk.sh.git
  ```
- Download the [ZIP archive](https://github.com/sylvaindethier/chalk.sh/archive/master.zip) and unzip

Then source the `chalk.sh/cli.sh` script:
```bash
$ source path/to/chalk.sh/cli.sh
```


## Usage

> `chalk.sh` provides exactly the same CLI usage as [`chalk-cli`](https://github.com/chalk/chalk-cli)

Make sure to source the `chalk.sh/cli.sh` script before running `chalk`

```bash
$ chalk --help

  Usage
    $ chalk <style> ... <string>
    $ echo <string> | chalk <style> ...

  Options
    --template, -t  Style template. The `~` character negates the style.

  Examples
    $ chalk red bold 'Unicorns & Rainbows'
    $ chalk -t '{red.bold Unicorns & Rainbows}'
    $ chalk -t '{red.bold Dungeons and Dragons {~bold.blue (with added fairies)}}'
```

See [`chalk` supported styles](https://github.com/chalk/chalk#styles)


## Template syntax

- `{red.bold unicorn}`
- `{red.bold unicorns} are {blue FUN!!!}`
- `{red.bold unicorn {blue.underline dancing}}`
- `{red red {~red normal}}`
- `{red hey\} still red} not red`
- `{red hey\\} not red`


## Related

- [chalk-cli](https://github.com/chalk/chalk-cli) - Original chalk CLI (NodeJS)
- [chalk](https://github.com/chalk/chalk) - Original chalk (NodeJS)


## License

MIT

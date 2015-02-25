# xcov

## Usage
Usage: xcov [OPTIONS]

Options:
  -help                     Show help
  -project PATH             Path to project
  -target TARGET            Target to use for coverage analysis
  -scheme NAME              Scheme to use for building
  -destination DESTINATION  Use the destination described by DESTINATION (a comma-separated set of key-value pairs describing the destination to use)
  -sdk VERSION              SDK to use for building (e.g. 8.0, 8.1)
  -configuration NAME       Configuration to use (e.g. Debug, Release)
  -output-format FORMAT     Output format (gcov or lcov)
  -clean                    Delete build directory (xcov-build)

## Install
Clone this repository and symlink `xcov` somewhere in your path:

```shell
$ git clone https://github.com/juliangrosshauser/xcov.git
$ ln -s $PWD/xcov/xcov /usr/local/bin/xcov
```

## Update
Just pull the updates into your local repository:

```shell
$ cd /path/to/xcov-repository
$ git pull
```

## License
[MIT](LICENSE)

# xcov
[![License](https://img.shields.io/badge/license-MIT-3f3f3f.svg)](http://choosealicense.com/licenses/mit)

**Xcode Code Coverage CLI**  
View the code coverage of your tests without changing the build settings of your Xcode project.

## Dependencies
* [`xcodebuild`](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/xcodebuild.1.html)
* [`gcov`](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/gcov.1.html) or [`lcov`](http://ltp.sourceforge.net/coverage/lcov.php)

If you have Xcode installed, `xcodebuild` and `gcov` will be available to you.  
You can install `lcov` with [Homebrew](http://brew.sh): `$ brew install lcov`  
`xcov` prefers `lcov`, because it produces HTML output.  
You can also use [CoverStory](https://code.google.com/p/coverstory) to view your code coverage.

## Usage
```
Usage: xcov [OPTIONS]

Options:
  -help                     Show help
  -project PATH             Path to project
  -workspace PATH           Path to workspace
  -target TARGET            Target to use for coverage analysis
  -scheme NAME              Scheme to use for building
  -destination DESTINATION  Use the destination described by DESTINATION (a comma-separated set of key-value pairs describing the destination to use)
  -sdk VERSION              SDK to use for building (e.g. 8.0, 8.1)
  -configuration NAME       Configuration to use (e.g. Debug, Release)
  -output-format FORMAT     Output format (gcov or lcov)
  -clean                    Delete build directory (xcov-build)
```

## Install
Clone this repository and symlink `xcov` somewhere in your `$PATH`:

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

homebrew-geoip
===============
[![Build Status](https://travis-ci.org/dutchcoders/homebrew-geoip.svg?branch=master)](https://travis-ci.org/dutchcoders/homebrew-geoip)

Homebrew formula for geoip.

## Usage

```bash
$ brew tap dutchcoders/homebrew-geoip
$ brew install gister
```

## Troubleshooting

* Make sure you're using the right formula.  `brew info gister` should have a
  From line similar to this:

  ```text
  From: https://github.com/dutchcoders/homebrew-gister/blob/master/Formula/geoip.rb
  ```

  If your formula points elsewhere, then you need to retap the gister formula.
  Do so with the following sequence of commands:

  ```text
  brew uninstall gister --force
  brew prune
  brew tap dutchcoders/homebrew-geoip
  brew tap --repair
  brew install geoip
  ```
* Run `brew update` — then try again.
* Run `brew doctor` — the doctor diagnoses common issues.
* You can create a gist log with `brew gist-logs geoip`.
* Use `--verbose` to get the verbose output, i.e. `brew install --verbose geoip`.
* Use `--debug` to be in the debug mode. In the debug mode, when failing, you
  can go into the interactive shell to check the building files before homebrew
  neutralizing them.

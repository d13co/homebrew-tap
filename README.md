# d13co/tap

Homebrew formulae for [dtalgorand](https://github.com/d13co/dt-algorand), a fork of the Algorand node (algod) with time travel: historical account and application state at past rounds.

## Install

Apple silicon, macOS 14 (Sonoma) or later:

```sh
brew install d13co/tap/dtalgorand
brew services start dtalgorand
```

The binaries are installed with a `dt` prefix (`dtalgod`, `dtgoal`, `dtkmd`, ...), so they don't clash with Algorand's own. The node's data directory is `$(brew --prefix)/var/dtalgorand`; `brew info dtalgorand` shows the details.

## Updates

The release workflow of [d13co/dt-algorand](https://github.com/d13co/dt-algorand) commits `Formula/dtalgorand.rb` here for each release. Don't edit it by hand: change the template in [installer/dtalgorand/homebrew](https://github.com/d13co/dt-algorand/tree/dtalgorand/installer/dtalgorand/homebrew) instead.

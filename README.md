# sauce-labs-check

Implements the [Sauce Labs Ruby example](https://docs.saucelabs.com/tutorials/ruby/) so that you
check your Sauce access *before* integrating it into your existing Rails app.

Sauce Labs used to maintain an example project that you could run [here](https://github.com/saucelabs/ruby-tutorial)
but it has since been [deprecated](https://github.com/saucelabs/docs/blob/master/markdown/tutorials/ruby.md)
in favour of a follow-along tutorial. It's somewhat painful to follow that everytime you just want
to run a simple app to make sure everything's working, so here's the implementation of their
[example](https://docs.saucelabs.com/tutorials/ruby/).

## Requirements

* I ran this on Ruby 2.1.5. If you don't have that, I highly recommend installing [rvm](http://rvm.io/)
and then `rvm install 2.1.5`
* Set up your environment variables by adding these lines to your `~/.bash_profile`, replacing them
with your values

```
export SAUCE_USERNAME=your_sauce_username
export SAUCE_ACCESS_KEY=your-sauce-access-key-from-your-account
```

## Installation

`git clone git@github.com:mence/sauce-labs-check.git`

`cd sauce-labs-check`

`bundle install`

## Running tests

`rake sauce:spec`
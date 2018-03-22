# Installing Jekyll on Mac OSX

## **DISCLAIMER:** This is just my experience. No guarantees that it will work for you

The following was successful on Mac OSX El Capitan (10.11.6)

```$ brew install ruby```

```$ brew install rbenv```

```$ rbenv init```

_\# Load rbenv automatically by appending<br/>_
_\# the following to ~/.bash_profile:_

_eval "$(rbenv init -)"_


```echo 'eval "$(rbenv init -)"' >> ~/.bash_profile```

**Close and reopen your terminal session in order to invoke the previous change.**

```$ curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash```

_Checking for `rbenv' in PATH:  /usr/local/bin/rbenv_
_Checking for rbenv shims in PATH: OK<br/>_
_Checking `rbenv install' support: /usr/local/bin/rbenv-install (ruby-build 20180224)<br/>_
_Counting installed Ruby versions: none<br/>_
  _There aren't any Ruby versions installed under `/Users/rwhitear/.rbenv/versions'.<br/>_
  _You can install Ruby versions like so: rbenv install 2.2.4<br/>_
_Checking RubyGems settings: OK<br/>_
_Auditing installed plugins: OK_

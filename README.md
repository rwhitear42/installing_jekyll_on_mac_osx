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

_Checking for 'rbenv' in PATH:  /usr/local/bin/rbenv_<br/>
_Checking for rbenv shims in PATH: OK<br/>_
_Checking 'rbenv install' support: /usr/local/bin/rbenv-install (ruby-build 20180224)<br/>_
_Counting installed Ruby versions: none<br/>_
  _There aren't any Ruby versions installed under `/Users/rwhitear/.rbenv/versions'.<br/>_
  _You can install Ruby versions like so: rbenv install 2.2.4<br/>_
_Checking RubyGems settings: OK<br/>_
_Auditing installed plugins: OK_

```$ brew upgrade rbenv ruby-build```

_Updating Homebrew..._

```$ rbenv install 2.5.0```

_ruby-build: use openssl from homebrew_<br/>
...<br/>
_Installed ruby-2.5.0 to /Users/rwhitear/.rbenv/versions/2.5.0_

```$ ruby --version```

_ruby 2.5.0p0 (2017-12-25 revision 61468) [x86_64-darwin15]_

```$ sudo gem install jekyll bundler```

_Fetching: public_suffix-3.0.2.gem (100%)_<br/>
...<br/>
_bundler's executable "bundle" conflicts with /usr/local/bin/bundle_<br/>
_Overwrite the executable? [yN]  y_<br/>
_bundler's executable "bundler" conflicts with /usr/local/bin/bundler_<br/>
_Overwrite the executable? [yN]  y_<br/>
_Successfully installed bundler-1.16.1_<br/>
_Parsing documentation for bundler-1.16.1_<br/>
_Installing ri documentation for bundler-1.16.1_<br/>
_Done installing documentation for bundler after 4 seconds_<br/>
_26 gems installed_

```$ jekyll new myblog```

_Running bundle install in /Users/rwhitear/Documents/GitHub/rwhitear42.github.io/myblog..._

**Enter sudo password when requested**

_New jekyll site installed in..._

```$ cd myblog/```

```$ bundle exec jekyll serve```

_Server address: http://127.0.0.1:4000/_
_Server running... press ctrl-c to stop._

# jlenv installer & doctor scripts

[![Build Status](https://travis-ci.com/jlenv/jlenv-installer.svg?branch=master)](https://travis-ci.com/jlenv/jlenv-installer)[![Codacy Badge](https://api.codacy.com/project/badge/Grade/dac67ef51fa34b25babb098b05145f72)](https://www.codacy.com/manual/taqtiqa-mark/jlenv-jlenv-installer?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jlenv/jlenv-installer&amp;utm_campaign=Badge_Grade)[![CodeFactor](https://www.codefactor.io/repository/github/jlenv/jlenv-installer/badge)](https://www.codefactor.io/repository/github/jlenv/jlenv-installer)

## jlenv-installer

The `jlenv-installer` script idempotently installs or updates jlenv on your
system. If Homebrew is detected, installation will proceed using `brew
install/upgrade`. Otherwise, jlenv is installed under `~/.jlenv`.

Additionally, [julia-build](https://github.com/jlenv/julia-build#readme) is also
installed if `jlenv install` is not already available.

```sh
# with curl
curl -fsSL https://raw.githubusercontent.com/jlenv/jlenv-installer/master/libexec/jlenv-installer | bash

# alternatively, with wget
wget -q https://raw.githubusercontent.com/jlenv/jlenv-installer/master/libexec/jlenv-installer -O- | bash
```

## jlenv-doctor

After the installation, a separate `jlenv-doctor` script is run to verify the
success of the installation and to detect common issues. You can run
`jlenv-doctor` on your machine separately to verify the state of your install:

```sh
# with curl
curl -fsSL https://raw.githubusercontent.com/jlenv/jlenv-installer/master/libexec/jlenv-doctor | bash

# alternatively, with wget
wget -q https://raw.githubusercontent.com/jlenv/jlenv-installer/master/libexec/jlenv-doctor -O- | bash
```

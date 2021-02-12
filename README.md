This repo is used to store specific versions of formulas.

The `brew extract` command can be used to create formula files from an old version or the latest version.

```
$ brew extract --help
Usage: brew extract [--version=] [--force] formula tap
```

Below is an example to create a formula file from the latest version of ninja
```
$ brew extract ninja gitlw/homebrew-versions

==> Tapping gitlw/versions
Cloning into '/home/linuxbrew/.linuxbrew/Homebrew/Library/Taps/gitlw/homebrew-versions'...
warning: You appear to have cloned an empty repository.
Tapped (17 files, 27.7KB).
==> Writing formula for ninja from revision HEAD to:
/home/linuxbrew/.linuxbrew/Homebrew/Library/Taps/gitlw/homebrew-versions/Formula/ninja@1.10.2.rb
```

Now that the `Formula/ninja@1.10.2.rb` file is created, you can simply commit it to this repo.

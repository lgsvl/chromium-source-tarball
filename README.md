# Chromium source tarball

Automatically generate source tarballs for Chromium releases channel, and upload
them to the
[releases](https://github.com/zcbenz/chromium-source-tarball/releases) page.

Unlike the offical source tarballs which only contains dependencies for Linux
that specified for Linux packagers, source tarballs in this repo includes the
dependencies of all platforms.

## Usage

### 1. Bootstrap

```bash
$ ./script/bootstrap git://downstream.repo.org/chromium.git
```

This will download upstream chromium repository, and set an alternate origin
for the passed parameter.

### 2. Generate the source tarball

```bash
$ ./script/sync 38.0.2125.101
```

Sync will accept as parameter any head that will be available in the provided
chromium repository. Then it will generate a tarball with the source code.

## License

The code of this project is published under public domain.

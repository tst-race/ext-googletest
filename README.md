# GoogleTest for RACE

This repo provides scripts to custom-build the
[GoogleTest library](https://github.com/google/googletest) for RACE.

## License

The GoogleTest library is licensed under the 3-Clause BSD license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

GoogleTest has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build GoogleTest.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-googletest.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-googletest
```

## Platforms

GoogleTest is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`

## How It Is Used

GoogleTest is used directly by the RACE core and exemplar plugins.

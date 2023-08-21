[![Build Status](https://github.com/hsel-netsys/iceflow/actions/workflows/build.yml/badge.svg)](https://github.com/hsel-netsys/iceflow/actions/workflows/build.yml)
[![Documentation Status](https://img.shields.io/github/actions/workflow/status/hsel-netsys/iceflow/doxygen-gh-pages.yml?label=docs&link=https%3A%2F%2Fhsel-netsys.github.io%2Ficeflow)](https://hsel-netsys.github.io/iceflow)
![License](https://img.shields.io/github/license/hsel-netsys/iceflow)

# IceFlow

This repository contains IceFlow, a stream processing library based on
Named-Data Networking (NDN) written in C++.
Besides the actual library, a number of applications are included in the
repository illustrating the use of IceFlow for a video processing use case.

<!-- TODO: Expand README -->

## Installation

Detailed installation instructions can be found in the file [Install.md](Install.md).

## Documentation

IceFlow's documentation can be found [here](https://hsel-netsys.github.io/iceflow).

If you Doxygen installed, you can generate the documentation locally using the
following commands in the repository's root directory:

```sh
cmake .
make docs
```

## Code Style

In order to achieve a consistent style, IceFlow's codebase is formatted using
`clang-format`.
After installing it (e.g., by using `brew install clang-format` on macOS) you
can format all source files by invoking the following commands:

```sh
cmake .
make format
```
The CI pipeline will assert that the codebase is always correctly
formatted and will fail otherwise.

## Static Analysis

IceFlow uses cppcheck to lint its source code.
To perform the linting step locally, use the following commands:

```sh
cmake .
make lint
```

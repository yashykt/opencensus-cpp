# OpenCensus - A stats collection and distributed tracing framework
[![Gitter chat][gitter-image]][gitter-url]

OpenCensus is a toolkit for collecting application performance and behavior data. It currently
includes an API for tracing.

The library is in alpha stage and the API is subject to change.

Please join [gitter](https://gitter.im/census-instrumentation/Lobby) for help or feedback on this
project.

[gitter-image]: https://badges.gitter.im/census-instrumentation/lobby.svg
[gitter-url]: https://gitter.im/census-instrumentation/lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge

This is not an officially supported Google product.

## Quickstart

Please refer to
[`trace/examples/span_example.cc`](opencensus/trace/examples/span_example.cc)

## Directory structure

* [`opencensus/`](opencensus) prefix to get `#include` paths like `opencensus/trace/span.h`
  * [`common/`](opencensus/common) - Provides common libraries and components for OpenCensus.
  * [`doc/`](opencensus/doc) - Documentation for our APIs, coding style, etc.
  * [`trace/`](opencensus/trace) - OpenCensus tracing API.

## Language support

* `libstdc++` is required.
* C++11 is required.
* [`absl`](https://github.com/abseil/abseil-cpp/) is used for its building blocks.
* [`googletest`](https://github.com/google/googletest/) is used for tests.
* [`benchmark`](https://github.com/google/benchmark/) is used for benchmarking.
* We do not depend on:
  * Boost
  * Exception handling
  * RTTI

## Compiler support

We are targeting the following compilers:

* gcc 4.8.1
* clang 3.4
* MSVC 19

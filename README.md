# Tauri-bazel-next-typescript

A small repository to demonstrate how to build a [Tauri](https://tauri.app/) project that is using [NextJS](https://nextjs.org/) + Typescript as a frontend framework with [Bazel](https://bazel.build/).

## Before running it

This project is using `git LFS`. After cloning it, remember to run the following commands

```bash
git lfs install
git lfs pull
```

## How to use

To run Tauri in development mode just run

```bash
bazel run :dev
```

To bundle your app just run

```bash
bazel run :bundle
```

If you are interested in running or building the frontend only run

```bash
bazel run :next-dev
bazel run :next-build
```

This has been tested successfully on macOS M1.

## Output

You can retrieve the output app from `dist/bin/bundle.sh.runfiles/app/src-tauri/target/release/bundle`

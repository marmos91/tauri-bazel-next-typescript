load("@npm//next:index.bzl", "next")
load("@npm//@tauri-apps/cli:index.bzl", "tauri")

next(
    name = "next-build",
    data = glob([
        "pages/**",
        "public/**",
        "styles/**",
    ]) + [
        "tsconfig.json",
    ],
    templated_args = ["build"],
)

next(
    name = "next-dev",
    data = glob([
        "pages/**",
        "public/**",
        "styles/**",
    ]) + [
        "tsconfig.json",
    ],
    templated_args = ["dev"],
)

tauri(
    name = "dev",
    data = glob(["**"]) + [
        "@npm//next",
    ],
    templated_args = [
        "dev",
    ],
)

tauri(
    name = "bundle",
    data = glob(["**"]) + [
        "@npm//next",
    ],
    templated_args = [
        "build",
    ],
)

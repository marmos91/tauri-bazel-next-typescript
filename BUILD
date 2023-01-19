load("@npm//next:index.bzl", "next")

exports_files([
    "tsconfig.json",
])

next(
    name = "build",
    data = glob([
        "pages/**",
        "public/**",
        "styles/**",
    ]) + [
        "package.json",
        "package-lock.json",
        "tsconfig.json",
        "next-env.d.ts",
        "next.config.js",
    ] + [
        "@npm//@next/font",
        "@npm//@types/node",
        "@npm//@types/react",
        "@npm//@types/react-dom",
        "@npm//eslint",
        "@npm//eslint-config-next",
        "@npm//react",
        "@npm//react-dom",
        "@npm//typescript",
    ],
    templated_args = ["build"],
)

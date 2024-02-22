load("@aspect_rules_ts//ts:defs.bzl", "ts_project")

ts_project(
    name = "good",
    srcs = [
        "script_1.ts",
        "a.ts"
    ],
    tsconfig = {},
    transpiler = 'tsc',
    root_dir = ".",
)

ts_project(
    name = "bad",
    srcs = [
        "script_2.ts",
        "//:b"
    ],
    tsconfig = {
        "rootDir": "..",
    },
    transpiler = 'tsc',
    root_dir = "..",
)

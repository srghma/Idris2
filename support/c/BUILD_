cc_library(
    name = "idris2_support",
    srcs = glob(["*.c"]) + select({
        "@platforms//os:windows": [
            "windows/win_utils.c",
            "windows/win_hack.c",
        ],
        "//conditions:default": [],
    }),
    hdrs = glob(["*.h"]),
    includes = ["."],
    copts = [
        "-O2",
        "-Wall",
        "-fPIC",
    ] + select({
        "@platforms//os:windows": [
            "-DWIN32_LEAN_AND_MEAN",
        ],
        "//conditions:default": [],
    }),
    linkopts = select({
        "@platforms//os:windows": ["-lws2_32"],
        "//conditions:default": [],
    }),
)

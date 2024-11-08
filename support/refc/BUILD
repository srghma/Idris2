cc_library(
    name = "idris2_refc",
    srcs = glob(["*.c"]),
    hdrs = glob(["*.h"]),
    includes = ["."],
    copts = [
        "-O2",
        "-Wall",
        "-fPIC",
    ],
)

# filegroup(
#     name = "install_files",
#     srcs = glob(["*.h"]) + [":idris2_support"],  # or idris2_refc for refc directory
# )

licenses(["notice"])

cc_library(
    name = "png",
    srcs = [
        "png.c",
        "pngerror.c",
        "pngget.c",
        "pngmem.c",
        "pngpread.c",
        "pngread.c",
        "pngrio.c",
        "pngrtran.c",
        "pngrutil.c",
        "pngset.c",
        "pngtrans.c",
        "pngwio.c",
        "pngwrite.c",
        "pngwtran.c",
        "pngwutil.c",
    ],
    hdrs = [
        "png.h",
        "pngconf.h",
        "pngdebug.h",
        "pnginfo.h",
        "pnglibconf.h",
        "pngpriv.h",
        "pngstruct.h",
    ],
    includes = ["."],
    linkopts =
        select({
            "@platforms//os:linux": ["-lm"],
            "//conditions:default": [],
        }),
    visibility = ["//visibility:public"],
    deps = ["@zlib//:zlib"],
)


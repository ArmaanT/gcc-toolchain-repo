load("@rules_foreign_cc//foreign_cc:defs.bzl", "configure_make")

package(default_visibility = ["//visibility:public"])

filegroup(
    name = "all_srcs",
    srcs = glob(["**"]),
)

configure_make(
    name = "zlib",
    copts = [
        "-fPIC",
    ],
    lib_source = ":all_srcs",
    out_shared_libs = [
        "libz.so",
        "libz.so.1",
        "libz.so.1.2.12",
    ],
    out_static_libs = [
        "libz.a",
    ],
)

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = [
        "bitmap.go",
        "interfaces.go",
        "utils.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/registry/core/service/allocator",
    tags = ["automanaged"],
)

go_test(
    name = "go_default_test",
    srcs = [
        "bitmap_test.go",
        "utils_test.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/registry/core/service/allocator",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//pkg/registry/core/service/allocator/storage:all-srcs",
    ],
    tags = ["automanaged"],
)

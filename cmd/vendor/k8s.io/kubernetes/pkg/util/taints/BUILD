package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["taints.go"],
    importpath = "k8s.io/kubernetes/pkg/util/taints",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/api/core/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/validation:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["taints_test.go"],
    importpath = "k8s.io/kubernetes/pkg/util/taints",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/spf13/pflag:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)

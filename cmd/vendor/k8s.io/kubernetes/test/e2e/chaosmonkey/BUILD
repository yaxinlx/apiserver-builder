package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["chaosmonkey.go"],
    importpath = "k8s.io/kubernetes/test/e2e/chaosmonkey",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/github.com/onsi/ginkgo:go_default_library"],
)

go_test(
    name = "go_default_test",
    srcs = ["chaosmonkey_test.go"],
    importpath = "k8s.io/kubernetes/test/e2e/chaosmonkey",
    library = ":go_default_library",
    tags = ["automanaged"],
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

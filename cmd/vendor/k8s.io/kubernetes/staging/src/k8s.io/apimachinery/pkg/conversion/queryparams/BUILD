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
        "convert.go",
        "doc.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apimachinery/pkg/conversion/queryparams",
    tags = ["automanaged"],
)

go_test(
    name = "go_default_xtest",
    srcs = ["convert_test.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apimachinery/pkg/conversion/queryparams_test",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/conversion/queryparams:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
    ],
)

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["install.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/metrics/pkg/apis/custom_metrics/install",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/apimachinery/announced:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apimachinery/registered:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//cmd/vendor/k8s.io/metrics/pkg/apis/custom_metrics:go_default_library",
        "//cmd/vendor/k8s.io/metrics/pkg/apis/custom_metrics/v1alpha1:go_default_library",
    ],
)

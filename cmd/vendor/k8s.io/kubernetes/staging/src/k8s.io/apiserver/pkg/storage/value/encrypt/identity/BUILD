package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["identity.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiserver/pkg/storage/value/encrypt/identity",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/k8s.io/apiserver/pkg/storage/value:go_default_library"],
)

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["trace.go"],
    importpath = "k8s.io/apiserver/pkg/util/trace",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/github.com/golang/glog:go_default_library"],
)

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["secretbox_test.go"],
    importpath = "k8s.io/apiserver/pkg/storage/value/encrypt/secretbox",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/k8s.io/apiserver/pkg/storage/value:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = ["secretbox.go"],
    importpath = "k8s.io/apiserver/pkg/storage/value/encrypt/secretbox",
    tags = ["automanaged"],
    deps = [
        "//vendor/golang.org/x/crypto/nacl/secretbox:go_default_library",
        "//cmd/vendor/k8s.io/apiserver/pkg/storage/value:go_default_library",
    ],
)

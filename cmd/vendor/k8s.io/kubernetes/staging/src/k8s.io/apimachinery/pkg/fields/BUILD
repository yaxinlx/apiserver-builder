package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = [
        "fields_test.go",
        "selector_test.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apimachinery/pkg/fields",
    library = ":go_default_library",
    tags = ["automanaged"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "fields.go",
        "requirements.go",
        "selector.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apimachinery/pkg/fields",
    tags = ["automanaged"],
    deps = ["//cmd/vendor/k8s.io/apimachinery/pkg/selection:go_default_library"],
)

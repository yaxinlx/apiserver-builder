package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["validation_test.go"],
    importpath = "k8s.io/apiserver/pkg/apis/audit/validation",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//vendor/k8s.io/apiserver/pkg/apis/audit:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = ["validation.go"],
    importpath = "k8s.io/apiserver/pkg/apis/audit/validation",
    tags = ["automanaged"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/api/validation:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/validation/field:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/apis/audit:go_default_library",
    ],
)

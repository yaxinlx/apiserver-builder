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
        "backoff_test.go",
        "throttle_test.go",
    ],
    importpath = "k8s.io/client-go/util/flowcontrol",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//vendor/k8s.io/apimachinery/pkg/util/clock:go_default_library"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "backoff.go",
        "throttle.go",
    ],
    importpath = "k8s.io/client-go/util/flowcontrol",
    tags = ["automanaged"],
    deps = [
        "//vendor/github.com/juju/ratelimit:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/clock:go_default_library",
        "//vendor/k8s.io/client-go/util/integer:go_default_library",
    ],
)

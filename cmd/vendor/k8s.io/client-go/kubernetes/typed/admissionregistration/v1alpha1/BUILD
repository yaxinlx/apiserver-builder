package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "admissionregistration_client.go",
        "doc.go",
        "externaladmissionhookconfiguration.go",
        "generated_expansion.go",
        "initializerconfiguration.go",
    ],
    importpath = "k8s.io/client-go/kubernetes/typed/admissionregistration/v1alpha1",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/api/admissionregistration/v1alpha1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/serializer:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes/scheme:go_default_library",
        "//cmd/vendor/k8s.io/client-go/rest:go_default_library",
    ],
)

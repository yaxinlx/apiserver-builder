package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "apiregistration_client.go",
        "apiservice.go",
        "doc.go",
        "generated_expansion.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/kube-aggregator/pkg/client/clientset_generated/clientset/typed/apiregistration/v1beta1",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/serializer:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//cmd/vendor/k8s.io/client-go/rest:go_default_library",
        "//cmd/vendor/k8s.io/kube-aggregator/pkg/apis/apiregistration/v1beta1:go_default_library",
        "//cmd/vendor/k8s.io/kube-aggregator/pkg/client/clientset_generated/clientset/scheme:go_default_library",
    ],
)

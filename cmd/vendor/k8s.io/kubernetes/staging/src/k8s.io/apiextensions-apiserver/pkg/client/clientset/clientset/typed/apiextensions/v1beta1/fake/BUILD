package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "fake_apiextensions_client.go",
        "fake_customresourcedefinition.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiextensions-apiserver/pkg/client/clientset/clientset/typed/apiextensions/v1beta1/fake",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apiextensions-apiserver/pkg/apis/apiextensions/v1beta1:go_default_library",
        "//cmd/vendor/k8s.io/apiextensions-apiserver/pkg/client/clientset/clientset/typed/apiextensions/v1beta1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//cmd/vendor/k8s.io/client-go/rest:go_default_library",
        "//cmd/vendor/k8s.io/client-go/testing:go_default_library",
    ],
)

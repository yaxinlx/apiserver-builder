package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "defaults.go",
        "doc.go",
        "generated.pb.go",
        "register.go",
        "types.go",
        "zz_generated.conversion.go",
        "zz_generated.deepcopy.go",
        "zz_generated.defaults.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apiextensions-apiserver/pkg/apis/apiextensions/v1beta1",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/gogo/protobuf/proto:go_default_library",
        "//cmd/vendor/k8s.io/apiextensions-apiserver/pkg/apis/apiextensions:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/conversion:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
    ],
)

filegroup(
    name = "go_default_library_protos",
    srcs = ["generated.proto"],
    visibility = ["//visibility:public"],
)

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
        "keystone.go",
    ],
    importpath = "k8s.io/apiserver/plugin/pkg/authenticator/password/keystone",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/gophercloud/gophercloud:go_default_library",
        "//vendor/github.com/gophercloud/gophercloud/openstack:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//cmd/vendor/k8s.io/apiserver/pkg/authentication/user:go_default_library",
        "//cmd/vendor/k8s.io/client-go/util/cert:go_default_library",
    ],
)

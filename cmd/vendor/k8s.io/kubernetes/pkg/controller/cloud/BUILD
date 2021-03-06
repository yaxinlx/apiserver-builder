package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["nodecontroller.go"],
    importpath = "k8s.io/kubernetes/pkg/controller/cloud",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/api/core/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//cmd/vendor/k8s.io/client-go/informers/core/v1:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes/scheme:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes/typed/core/v1:go_default_library",
        "//cmd/vendor/k8s.io/client-go/tools/cache:go_default_library",
        "//cmd/vendor/k8s.io/client-go/tools/record:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api/v1/node:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/client/retry:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/cloudprovider:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/kubelet/apis:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/util/node:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/plugin/pkg/scheduler/algorithm:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["nodecontroller_test.go"],
    importpath = "k8s.io/kubernetes/pkg/controller/cloud",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/api/core/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//cmd/vendor/k8s.io/client-go/informers:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes/fake:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes/scheme:go_default_library",
        "//cmd/vendor/k8s.io/client-go/tools/record:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/cloudprovider:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/cloudprovider/providers/fake:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/controller:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/controller/node/testutil:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/kubelet/apis:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/plugin/pkg/scheduler/algorithm:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)

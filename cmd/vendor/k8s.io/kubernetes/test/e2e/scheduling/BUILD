package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "events.go",
        "framework.go",
        "nvidia-gpus.go",
        "opaque_resource.go",
        "predicates.go",
        "priorities.go",
        "rescheduler.go",
    ],
    importpath = "k8s.io/kubernetes/test/e2e/scheduling",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/onsi/ginkgo:go_default_library",
        "//cmd/vendor/github.com/onsi/gomega:go_default_library",
        "//vendor/github.com/stretchr/testify/assert:go_default_library",
        "//cmd/vendor/k8s.io/api/core/v1:go_default_library",
        "//cmd/vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/yaml:go_default_library",
        "//cmd/vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api/v1/helper:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api/v1/pod:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/util/system:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/plugin/pkg/scheduler/algorithm/priorities/util:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/test/e2e/common:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/test/e2e/framework:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/test/utils:go_default_library",
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

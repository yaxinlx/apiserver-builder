package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "procfs.go",
        "procfs_fake.go",
        "procfs_unsupported.go",
    ] + select({
        "@io_bazel_rules_go//go/platform:linux_amd64": [
            "procfs_linux.go",
        ],
        "//conditions:default": [],
    }),
    importpath = "k8s.io/kubernetes/pkg/util/procfs",
    tags = ["automanaged"],
    deps = select({
        "@io_bazel_rules_go//go/platform:linux_amd64": [
            "//cmd/vendor/github.com/golang/glog:go_default_library",
            "//cmd/vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        ],
        "//conditions:default": [],
    }),
)

go_test(
    name = "go_default_test",
    srcs = select({
        "@io_bazel_rules_go//go/platform:linux_amd64": [
            "procfs_linux_test.go",
        ],
        "//conditions:default": [],
    }),
    data = [
        "example_proc_cgroup",
    ],
    importpath = "k8s.io/kubernetes/pkg/util/procfs",
    library = ":go_default_library",
    tags = [
        "automanaged",
    ],
    deps = select({
        "@io_bazel_rules_go//go/platform:linux_amd64": [
            "//vendor/github.com/stretchr/testify/assert:go_default_library",
        ],
        "//conditions:default": [],
    }),
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

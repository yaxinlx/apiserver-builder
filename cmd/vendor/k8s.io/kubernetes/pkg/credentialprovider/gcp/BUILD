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
        "jwt.go",
        "metadata.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/credentialprovider/gcp",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/github.com/spf13/pflag:go_default_library",
        "//vendor/golang.org/x/oauth2:go_default_library",
        "//vendor/golang.org/x/oauth2/google:go_default_library",
        "//vendor/golang.org/x/oauth2/jwt:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/credentialprovider:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "jwt_test.go",
        "metadata_test.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/credentialprovider/gcp",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/credentialprovider:go_default_library",
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

load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["discovery.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/coreos/etcd/discovery",
    importpath = "github.com/coreos/etcd/discovery",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/coreos/etcd/client:go_default_library",
        "//vendor/github.com/coreos/etcd/pkg/transport:go_default_library",
        "//vendor/github.com/coreos/etcd/pkg/types:go_default_library",
        "//vendor/github.com/coreos/pkg/capnslog:go_default_library",
        "//vendor/github.com/jonboulle/clockwork:go_default_library",
        "//vendor/golang.org/x/net/context:go_default_library",
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
    visibility = ["//visibility:public"],
)

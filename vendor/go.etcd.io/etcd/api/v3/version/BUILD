load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["version.go"],
    importmap = "k8s.io/cloud-provider-gcp/vendor/go.etcd.io/etcd/api/v3/version",
    importpath = "go.etcd.io/etcd/api/v3/version",
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/coreos/go-semver/semver:go_default_library"],
)

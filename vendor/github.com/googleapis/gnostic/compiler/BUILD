load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "context.go",
        "error.go",
        "extensions.go",
        "helpers.go",
        "main.go",
        "reader.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/github.com/googleapis/gnostic/compiler",
    importpath = "github.com/googleapis/gnostic/compiler",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/protobuf/proto:go_default_library",
        "//vendor/github.com/golang/protobuf/ptypes/any:go_default_library",
        "//vendor/github.com/googleapis/gnostic/extensions:go_default_library",
        "//vendor/github.com/googleapis/gnostic/jsonschema:go_default_library",
        "//vendor/gopkg.in/yaml.v3:go_default_library",
    ],
)

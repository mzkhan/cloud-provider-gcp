load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "deepcopy.go",
        "doc.go",
        "helpers.go",
        "register.go",
        "types.go",
        "types_jsonschema.go",
        "zz_generated.deepcopy.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/k8s.io/apiextensions-apiserver/pkg/apis/apiextensions",
    importpath = "k8s.io/apiextensions-apiserver/pkg/apis/apiextensions",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
    ],
)

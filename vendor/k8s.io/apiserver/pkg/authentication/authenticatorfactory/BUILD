load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "delegating.go",
        "loopback.go",
        "metrics.go",
        "requestheader.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/k8s.io/apiserver/pkg/authentication/authenticatorfactory",
    importpath = "k8s.io/apiserver/pkg/authentication/authenticatorfactory",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/authenticator:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/group:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/anonymous:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/bearertoken:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/headerrequest:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/union:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/websocket:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/request/x509:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/token/cache:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/token/tokenfile:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/user:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server/dynamiccertificates:go_default_library",
        "//vendor/k8s.io/apiserver/plugin/pkg/authenticator/token/webhook:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/typed/authentication/v1:go_default_library",
        "//vendor/k8s.io/component-base/metrics:go_default_library",
        "//vendor/k8s.io/component-base/metrics/legacyregistry:go_default_library",
        "//vendor/k8s.io/kube-openapi/pkg/validation/spec:go_default_library",
    ],
)

load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "dir_unix.go",
        "dir_windows.go",
        "doc.go",
        "fileutil.go",
        "lock.go",
        "lock_flock.go",
        "lock_linux.go",
        "lock_plan9.go",
        "lock_solaris.go",
        "lock_unix.go",
        "lock_windows.go",
        "preallocate.go",
        "preallocate_darwin.go",
        "preallocate_unix.go",
        "preallocate_unsupported.go",
        "purge.go",
        "read_dir.go",
        "sync.go",
        "sync_darwin.go",
        "sync_linux.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/go.etcd.io/etcd/client/pkg/v3/fileutil",
    importpath = "go.etcd.io/etcd/client/pkg/v3/fileutil",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/go.uber.org/zap:go_default_library",
    ] + select({
        "@io_bazel_rules_go//go/platform:android": [
            "//vendor/golang.org/x/sys/unix:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:darwin": [
            "//vendor/golang.org/x/sys/unix:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:ios": [
            "//vendor/golang.org/x/sys/unix:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:linux": [
            "//vendor/golang.org/x/sys/unix:go_default_library",
        ],
        "//conditions:default": [],
    }),
)

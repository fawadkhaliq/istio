load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    visibility = ["//visibility:private"],
    deps = [
        "//pkg/log:go_default_library",
        "//security/integration/utils:go_default_library",
        "//security/pkg/cmd:go_default_library",
        "//security/pkg/pki/ca/controller:go_default_library",
        "//security/pkg/pki/testutil:go_default_library",
        # TODO(nmittler): Remove this
        "@com_github_golang_glog//:go_default_library",
        "@com_github_spf13_cobra//:go_default_library",
        "@io_k8s_api//core/v1:go_default_library",
        "@io_k8s_apimachinery//pkg/apis/meta/v1:go_default_library",
        "@io_k8s_client_go//kubernetes:go_default_library",
    ],
)

go_binary(
    name = "integration",
    library = ":go_default_library",
    visibility = ["//visibility:public"],
)

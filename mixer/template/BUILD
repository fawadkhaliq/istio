# gazelle:exclude template.gen.go

load("@io_bazel_rules_go//go:def.bzl", "go_library")

package(default_visibility = ["//visibility:public"])

load("//mixer/tools/codegen:generate.bzl", "mixer_supported_template_library")

mixer_supported_template_library(
    name = "go_default_library",
    packages = {
        "//mixer/adapter/servicecontrol/template/servicecontrolreport:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/adapter/servicecontrol/template/servicecontrolreport",
        "//mixer/template/apikey:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/apikey",
        "//mixer/template/authorization:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/authorization",
        "//mixer/template/checknothing:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/checknothing",
        "//mixer/adapter/kubernetesenv/template:descriptor_set": "istio.io/istio/mixer/adapter/kubernetesenv/template",
        "//mixer/template/listentry:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/listentry",
        "//mixer/template/logentry:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/logentry",
        "//mixer/template/metric:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/metric",
        "//mixer/template/quota:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/quota",
        "//mixer/template/reportnothing:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/reportnothing",
        "//mixer/template/tracespan:go_default_library_proto.descriptor_set": "istio.io/istio/mixer/template/tracespan",
    },
    deps = [
        "//mixer/adapter/kubernetesenv/template:go_default_library",
        "//mixer/adapter/servicecontrol/template/servicecontrolreport:go_default_library",
        "//mixer/template/apikey:go_default_library",
        "//mixer/template/authorization:go_default_library",
        "//mixer/template/checknothing:go_default_library",
        "//mixer/template/listentry:go_default_library",
        "//mixer/template/logentry:go_default_library",
        "//mixer/template/metric:go_default_library",
        "//mixer/template/quota:go_default_library",
        "//mixer/template/reportnothing:go_default_library",
        "//mixer/template/tracespan:go_default_library",
    ],
)

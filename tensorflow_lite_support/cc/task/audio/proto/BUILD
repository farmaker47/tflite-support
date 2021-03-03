load("//tools/build_defs/proto/cpp:cc_proto_library.bzl", "cc_proto_library")

package(
    default_visibility = [
        "//visibility:public",
    ],
    licenses = ["notice"],  # Apache 2.0
)

# Common audio protos.

proto_library(
    name = "classifications_proto",
    srcs = ["classifications.proto"],
    cc_api_version = 2,
    deps = [
        ":class_proto",
    ],
)

cc_proto_library(
    name = "classifications_cc_proto",
    deps = [
        ":classifications_proto",
    ],
)

proto_library(
    name = "class_proto",
    srcs = ["class.proto"],
    cc_api_version = 2,
)

cc_proto_library(
    name = "class_cc_proto",
    deps = [
        ":class_proto",
    ],
)

# AudioClassifier protos.

proto_library(
    name = "audio_classifier_options_proto",
    srcs = ["audio_classifier_options.proto"],
    cc_api_version = 2,
    deps = [
        "//tensorflow_lite_support/cc/task/core/proto:external_file_proto",
    ],
)

cc_proto_library(
    name = "audio_classifier_options_cc_proto",
    deps = [
        ":audio_classifier_options_proto",
    ],
)

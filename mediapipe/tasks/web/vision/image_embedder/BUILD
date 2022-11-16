# This contains the MediaPipe Image Embedder Task.
#
# This task performs embedding extraction on images.

load("//mediapipe/framework/port:build_config.bzl", "mediapipe_ts_declaration", "mediapipe_ts_library")

package(default_visibility = ["//mediapipe/tasks:internal"])

licenses(["notice"])

mediapipe_ts_library(
    name = "image_embedder",
    srcs = ["image_embedder.ts"],
    deps = [
        ":image_embedder_types",
        "//mediapipe/framework:calculator_jspb_proto",
        "//mediapipe/framework:calculator_options_jspb_proto",
        "//mediapipe/tasks/cc/components/containers/proto:embeddings_jspb_proto",
        "//mediapipe/tasks/cc/vision/image_embedder/proto:image_embedder_graph_options_jspb_proto",
        "//mediapipe/tasks/web/components/containers:embedding_result",
        "//mediapipe/tasks/web/components/processors:base_options",
        "//mediapipe/tasks/web/components/processors:embedder_options",
        "//mediapipe/tasks/web/components/processors:embedder_result",
        "//mediapipe/tasks/web/core",
        "//mediapipe/tasks/web/core:embedder_options",
        "//mediapipe/tasks/web/core:task_runner",
        "//mediapipe/tasks/web/vision/core:running_mode",
        "//mediapipe/web/graph_runner:wasm_mediapipe_lib_ts",
    ],
)

mediapipe_ts_declaration(
    name = "image_embedder_types",
    srcs = [
        "image_embedder_options.d.ts",
        "image_embedder_result.d.ts",
    ],
    deps = [
        "//mediapipe/tasks/web/components/containers:embedding_result",
        "//mediapipe/tasks/web/core",
        "//mediapipe/tasks/web/core:embedder_options",
        "//mediapipe/tasks/web/vision/core:running_mode",
    ],
)
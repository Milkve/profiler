load("@npm_angular_bazel//:index.bzl", "ng_module")
load("@io_bazel_rules_sass//:defs.bzl", "sass_binary")

package(default_visibility = ["//frontend:internal"])

ng_module(
    name = "memory_timeline_graph",
    srcs = [
        "memory_timeline_graph.ts",
        "memory_timeline_graph_module.ts",
    ],
    assets = [
        ":memory_timeline_graph_css",
        "memory_timeline_graph.ng.html",
    ],
    deps = [
        "@npm//@angular/core",
        "@org_xprof//frontend/app/common/angular:angular_material_card",
        "@org_xprof//frontend/third_party/google_visualization",
        "@org_xprof//frontend/app/common/interfaces",
    ],
)



sass_binary(
    name = "memory_timeline_graph_css",
    src = "memory_timeline_graph.scss",

    sourcemap = False,

    deps = [
        "@org_xprof//frontend/app/styles:common",
    ],
)

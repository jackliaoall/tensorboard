package(default_visibility = ["//tensorboard:internal"])

load("//tensorboard/defs:defs.bzl", "tensorboard_webcomponent_library")
load("//tensorboard/defs:web.bzl", "tf_web_library")

licenses(["notice"])  # Apache 2.0

tf_web_library(
    name = "tf_graph_info",
    srcs = [
        "tf-graph-info.html",
        "tf-node-info.html",
        "tf-node-list-item.html",
    ],
    path = "/tf-graph-info",
    deps = [
        "//tensorboard/components/tf_dashboard_common",
        "//tensorboard/components/tf_imports:polymer",
        "//tensorboard/plugins/graph/tf_graph_common",
        "//tensorboard/plugins/graph/tf_graph_debugger_data_card",
        "//tensorboard/plugins/graph/tf_graph_op_compat_card",
        "@org_polymer_iron_collapse",
        "@org_polymer_iron_list",
        "@org_polymer_paper_button",
        "@org_polymer_paper_icon_button",
        "@org_polymer_paper_item",
        "@org_polymer_paper_material",
        "@org_polymer_paper_slider",
        "@org_polymer_paper_spinner",
    ],
)

tensorboard_webcomponent_library(
    name = "legacy",
    srcs = [":tf_graph_info"],
    destdir = "tf-graph-info",
    deps = [
        "//tensorboard/components/tf_dashboard_common:legacy",
        "//tensorboard/components/tf_imports:polymer_lib",
        "//tensorboard/plugins/graph/tf_graph_common:legacy",
        "//tensorboard/plugins/graph/tf_graph_debugger_data_card:legacy",
        "//tensorboard/plugins/graph/tf_graph_op_compat_card:legacy",
        "//third_party/javascript/polymer/v2/iron-collapse:lib",
        "//third_party/javascript/polymer/v2/iron-list:lib",
        "//third_party/javascript/polymer/v2/paper-button:lib",
        "//third_party/javascript/polymer/v2/paper-icon-button:lib",
        "//third_party/javascript/polymer/v2/paper-item:lib",
        "//third_party/javascript/polymer/v2/paper-material:lib",
        "//third_party/javascript/polymer/v2/paper-slider:lib",
        "//third_party/javascript/polymer/v2/paper-spinner:lib",
    ],
)

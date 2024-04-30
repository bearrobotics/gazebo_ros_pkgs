load(
    "@com_github_mvukov_rules_ros//ros:interfaces.bzl",
    "cc_ros_interface_library",
    "ros_interface_library",
)

ros_interface_library(
    name = "gazebo_msgs",
    srcs = glob([
        "msg/*",
        "srv/*",
    ]),
    visibility = [
        "//visibility:public",
    ],
    deps = [
        "@ros_common_msgs//:geometry_msgs",
        "@ros_std_msgs//:std_msgs",
        "@ros_common_msgs//:trajectory_msgs",
    ],
)

cc_ros_interface_library(
    name = "cc_gazebo_msgs",
    visibility = [
        "//visibility:public",
    ],
    deps = [":gazebo_msgs"],
)
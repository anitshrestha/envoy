package(default_visibility = ["//visibility:public"])

load("//bazel:envoy_build_system.bzl", "envoy_cc_library")

envoy_cc_library(
    name = "client_ssl_auth_lib",
    srcs = ["client_ssl_auth.cc"],
    hdrs = ["client_ssl_auth.h"],
    deps = [
        "//include/envoy/network:connection_includes",
        "//include/envoy/server:instance_includes",
        "//source/common/filter/auth:client_ssl_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)

envoy_cc_library(
    name = "echo_lib",
    srcs = ["echo.cc"],
    deps = [
        "//include/envoy/network:connection_includes",
        "//source/common/filter:echo_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)

envoy_cc_library(
    name = "http_connection_manager_lib",
    srcs = ["http_connection_manager.cc"],
    hdrs = ["http_connection_manager.h"],
    deps = [
        "//include/envoy/filesystem:filesystem_includes",
        "//include/envoy/http:filter_includes",
        "//include/envoy/network:connection_includes",
        "//include/envoy/server:instance_includes",
        "//include/envoy/server:options_includes",
        "//include/envoy/stats:stats_includes",
        "//source/common/common:logger_lib",
        "//source/common/http:conn_manager_lib",
        "//source/common/http:date_provider_lib",
        "//source/common/http:utility_lib",
        "//source/common/http/access_log:access_log_lib",
        "//source/common/http/http1:codec_lib",
        "//source/common/http/http2:codec_lib",
        "//source/common/json:config_schemas_lib",
        "//source/common/json:json_loader_lib",
        "//source/common/router:rds_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)

envoy_cc_library(
    name = "mongo_proxy_lib",
    srcs = ["mongo_proxy.cc"],
    hdrs = ["mongo_proxy.h"],
    deps = [
        "//include/envoy/network:connection_includes",
        "//include/envoy/server:instance_includes",
        "//source/common/json:config_schemas_lib",
        "//source/common/mongo:proxy_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)

envoy_cc_library(
    name = "ratelimit_lib",
    srcs = ["ratelimit.cc"],
    hdrs = ["ratelimit.h"],
    deps = [
        "//include/envoy/network:connection_includes",
        "//source/common/filter:ratelimit_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)

envoy_cc_library(
    name = "redis_proxy_lib",
    srcs = ["redis_proxy.cc"],
    hdrs = ["redis_proxy.h"],
    deps = [
        "//source/common/redis:codec_lib",
        "//source/common/redis:command_splitter_lib",
        "//source/common/redis:conn_pool_lib",
        "//source/common/redis:proxy_filter_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)

envoy_cc_library(
    name = "tcp_proxy_lib",
    srcs = ["tcp_proxy.cc"],
    hdrs = ["tcp_proxy.h"],
    deps = [
        "//include/envoy/network:connection_includes",
        "//include/envoy/server:instance_includes",
        "//source/common/filter:tcp_proxy_lib",
        "//source/server:configuration_lib",
    ],
    alwayslink = 1,
)
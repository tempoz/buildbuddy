load("//rules/typescript:index.bzl", "ts_library")

package(default_visibility = ["//enterprise:__subpackages__"])

exports_files(["registry.css"])

ts_library(
    name = "registry",
    srcs = ["registry.tsx"],
    deps = [
        "//:node_modules/@types/react",
        "//:node_modules/react",
        "//app/components/spinner",
        "//app/errors:error_service",
        "//app/service:rpc_service",
        "//enterprise/app/registry:image",
        "//enterprise/app/registry:repository",
        "//proto:registry_ts_proto",
    ],
)

ts_library(
    name = "image",
    srcs = ["image.tsx"],
    deps = [
        "//:node_modules/@types/react",
        "//:node_modules/lucide-react",
        "//:node_modules/react",
        "//app/util:clipboard",
        "//app/util:react",
        "//proto:registry_ts_proto",
    ],
)

ts_library(
    name = "repository",
    srcs = ["repository.tsx"],
    deps = [
        "//:node_modules/@types/react",
        "//:node_modules/react",
        "//app/components/link",
        "//proto:registry_ts_proto",
    ],
)

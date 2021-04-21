# Public notice: this file is for internal documentation, testing, and
# reference only. Note that repo maintainers can freely change any part of the
# repository code at any time.
load("@io_bazel_rules_docker//container:container.bzl", "container_image")

# This example runs a python program that walks the filesystem under "/etc" and prints every filename.
container_image(
    name = "cloudsec_distroless_debug",
    base = "@distroless_base_debug//image",
    env = {
        "APP": "First BAZEL IMAGE",
        "xyz": "321",
    },
)


load("@io_bazel_rules_docker//container:container.bzl", "container_image")


#load("@io_bazel_rules_docker//python:image.bzl", "py3_image")

load("@io_bazel_rules_docker//cc:image.bzl", "cc_image")

cc_image(
    name = "cc_image",
    srcs = ["cc_image.cc"],
    deps = [":cc_image_library"],
)

container_image(
    name = "cloudsec_distroless_debug",
    base = ":cc_image",
    env = {
        "APP": "First BAZEL IMAGE",
        "xyz": "321",
    },
)

#container_image(
    #name = "cloudsec_distroless",
    #base = "@distroless_base//image",
    #env = {
        #"APP": "First BAZEL IMAGE",
        #"xyz": "321",
    #},
#)

#container_image(
    #name = "app",
    ## References container_pull from WORKSPACE (above)
    ##base = "@java_base//image",
    #files = ["//java/com/example/app:Hello_deploy.jar"],
    #cmd = ["Hello_deploy.jar"]
#)

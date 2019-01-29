load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "f22f9779199f586ef12a7cf89439fc620cae553bb56ec1602faee6e4931c7901",
    strip_prefix = "rules_go-cbdc86a7d89eadb4ab5cc700f672a1c74e20e996",
    url = "https://github.com/bazelbuild/rules_go/archive/cbdc86a7d89eadb4ab5cc700f672a1c74e20e996.tar.gz",
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "f490124dd4b97c136cb8565f3aeefc2f2c1736afda7728b9b227b2b8aeadc88c",
    strip_prefix = "bazel-gazelle-44ce230b3399a5d4472198740358fcd825b0c3c9",
    url = "https://github.com/bazelbuild/bazel-gazelle/archive/44ce230b3399a5d4472198740358fcd825b0c3c9.tar.gz",
)

load("@io_bazel_rules_go//go:def.bzl", "go_register_toolchains", "go_rules_dependencies")

go_rules_dependencies()

go_register_toolchains(
    # nogo = "@//:nogo",
)

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies", "go_repository")

gazelle_dependencies()
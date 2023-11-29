load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# Add the rules_python repository first
http_archive(
    name = "rules_python",
    urls = ["https://github.com/bazelbuild/rules_python/archive/refs/tags/4.1.0.tar.gz"],
    strip_prefix = "rules_python-4.1.0",
)

# Now load the rules_python repositories
load("@rules_python//python:repositories.bzl", "py_repositories")

# Load other dependencies
py_repositories()

# Now you can use the rules_python and other dependencies
load("@rules_python//python:defs.bzl", "py_binary")

# Add your Python targets and rules here

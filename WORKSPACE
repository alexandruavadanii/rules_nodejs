workspace(name = "io_bazel_rules_typescript")

load("//:defs.bzl", "node_repositories", "yarn_install")

# Install a hermetic version of node
# After this is run, a label @io_bazel_typescript_node//:bin/node will exist
node_repositories()

# Install yarn, and run yarn install to create node_modules.
# Also creates the BUILD file under node_modules.
yarn_install(package_json = "//:package.json")

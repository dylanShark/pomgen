java_library(
    name = "parent1",
    srcs = glob(["src/main/java/**/*.java"]),
    # these deps get pulled into the pom generated for *this* package
    deps = ["//examples/skip-artifact-generation/passthrough:set1"],
    runtime_deps = ["@maven//:org_antlr_stringtemplate"],
)

java_binary(
    name = "Main",
    srcs = glob(["src/**/*.java"]),
    deps = [":parent1"],
)
    

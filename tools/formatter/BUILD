package(default_visibility = ["//visibility:public"])

java_binary(
    name = "formatter",
    srcs = ["FormatterTool.java"],
    main_class = "com.google.startupos.tools.formatter.FormatterTool",
    runtime_deps = [
        "//tools:buildifier",
        # TODO: Current downloaded file is 292mb. Find a smaller source for the formatter.
        #"//tools:clang_format",
    ],
    deps = [
        "//common/flags",
        "//third_party/maven/com/google/flogger:flogger_system_backend",
        "//third_party/maven/com/google/googlejavaformat:google_java_format",
        "//third_party/maven/com/google/guava",
        "//third_party/maven/org/slf4j:slf4j_simple",
    ],
)

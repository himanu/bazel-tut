py_library(
    name = "calculator1",
    srcs = ["calculator.py"],
    # visibility = ["//visibility:public"],
)

py_test(
    name = "index_test",
    srcs = ["index_test.py"],
    main = "index_test.py",  
    deps = [
        "//calculator:calculator1",
    ],
)


## LEARNING BAZEL

1. BAZEL is a build automation tool
2. We define instructions/target in `BUILD` file.
3. Now bazel can build according to those instruction.

Bazel has also a concept of Package. Folder in which the `BUILD` file is present is known as package.
So in current repo, projectA is a package.

## WORKSPACE
1. `WORKSPACE` file can be used to bring external dependencies in our project


## SOME RULES
### `py_library`
1. defines reusable code that can be imported by other targets
2. Does not produce an executable
3. Can be a dependency of `py_binary` or other `py_library` targets.

### `py_binary`
1. Defines an executable Python program.
2. Requires a `main` python file (typically specified in srcs or main attribute).
3. Can depend on `py_library` targets for code reuse.
4. Produces an executable you can run using `bazel run`.

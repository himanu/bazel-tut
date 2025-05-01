### Learnings

1. If I run test file using `python3 index_test.py`, it would fail.
2. Because the import statement is relative to root.
3. Even if i run it from root, then also it would fail

1. But if run `index_test` target using bazel,
2. the test cases would be executed successfully.
3. Intially I was using `from calculator import Calculator` then `bazel test` was failing
4. But `python3 index_test.py` was running.

**Conclustion**
1. So my understanding is that
2. If we want to use bazel, then import statement have path relative to bazel workspace.
3. And Bazel workspace is the directory where `WORKSPACE` file is created.
4. It our case, it is Monorepo directory.


1. If also need to provide calculator as a dependency in the test target.
2. Otherwise it would fail.
3. For defining a dependency, we created a library.



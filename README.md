# Reproducer for [bazelbuild/bazel#12545](https://github.com/bazelbuild/bazel/issues/12545)

Successful run:

```
USE_BAZEL_VERSION=3.6.0 bazelisk test //:test --run_under=@bazel_12545//:wrapper.sh
```

Fails in 3.7.x:

```
USE_BAZEL_VERSION=3.7.0 bazelisk test //:test --run_under=@bazel_12545//:wrapper.sh
```


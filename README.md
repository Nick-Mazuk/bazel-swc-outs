# SWC Bazel outs

Using `rules_swc` with `ts_project` doesn't allow you to use `js_outs`.

## Reproduction steps

```
bazel build //:test
```

Then, look at `./bazel-bin`, and see that there's a file named `in.js`, not the expected `out.mjs`.

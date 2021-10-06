mdx-rule-test
=============

In dune `(mdx 0.1)` seems to be seriously broken. Try this:

```sh
dune runtest
```

1. `exists.md` gets evaluated fine, so it works
2. `generated.md` is never generated, the rule never triggers
3. `missing.md` is never checked, so its absence is never noticed. Probably
   `generated.md` runs into the same issue.

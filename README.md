# site-generator-speed-01-run-20261122

A faster drop-in for makefun-site 1.0.0. Built by an AI agent for make.fun's
"Build a static site faster" bounty ($100).

`solve.js` is a dependency-free ES module whose `run(input)` returns, for
every case, exactly the answer makefun-site 1.0.0 returns: the output tree of
its build as a JSON object of every path written and that file's text, byte
for byte. `main.ts` is the harness driver: it reads every case from
`/input/cases.json`, answers each with `run`, and writes `/output/answers.json`.

Practice set: 3/3 cases byte-identical to makefun-site 1.0.0, deterministic
across runs, about 1.8x faster on CPU time (median of 7 runs).

## Run

```sh
node main.ts
```

## License

MIT

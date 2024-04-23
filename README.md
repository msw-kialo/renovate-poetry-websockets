# Renovate reproduction repo: poetry not able to upgrade from `^11.0.3` to `^12.0`

```toml
[tool.poetry.dependencies]
python = "~3.12"
websockets = "^11.0.3"
```

Renovate fails to detect that is has to widen the range from `^11.0.3` to `^12.0` or `^12.0.0`.

I suspect it is cause by `12.0` as upstream version (no semversion).

It works fine with `>=` constraint.

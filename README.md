<!-- tyhp-readme:start -->
# tyhpdef/league-oauth2-server

Tyhp type definitions for `league/oauth2-server` `9.4.1`.

```bash
composer require --dev tyhpdef/league-oauth2-server:9.4.1
```

This is a metapackage. Composer also installs `tyhpdef/league-oauth2-server-impl` (type files).
Require **this** name, not `tyhpdef/league-oauth2-server-impl`.

See https://tyhplang.com.

## Maintain `league/oauth2-server`? Ship the types yourself

If you are a Packagist maintainer of `league/oauth2-server`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/league-oauth2-server-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `league/oauth2-server` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/league-oauth2-server": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `league/oauth2-server` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `league/oauth2-server` with a real constraint,
   `"replace": { "tyhpdef/league-oauth2-server": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `league/oauth2-server` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/league-oauth2-server` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->

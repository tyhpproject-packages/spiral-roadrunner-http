<!-- tyhp-readme:start -->
# tyhpdef/spiral-roadrunner-http

Tyhp type definitions for `spiral/roadrunner-http` `4.1.0`.

```bash
composer require --dev tyhpdef/spiral-roadrunner-http:4.1.0
```

This is a metapackage. Composer also installs `tyhpdef/spiral-roadrunner-http-impl` (type files).
Require **this** name, not `tyhpdef/spiral-roadrunner-http-impl`.

See https://tyhplang.com.

## Maintain `spiral/roadrunner-http`? Ship the types yourself

If you are a Packagist maintainer of `spiral/roadrunner-http`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/spiral-roadrunner-http-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `spiral/roadrunner-http` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/spiral-roadrunner-http": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `spiral/roadrunner-http` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `spiral/roadrunner-http` with a real constraint,
   `"replace": { "tyhpdef/spiral-roadrunner-http": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `spiral/roadrunner-http` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/spiral-roadrunner-http` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->

<!-- tyhp-readme:start -->
# tyhpdef/doctrine-doctrine-bundle

Tyhp type definitions for `doctrine/doctrine-bundle` `3.3.2`.

```bash
composer require --dev tyhpdef/doctrine-doctrine-bundle:3.3.2
```

This is a metapackage. Composer also installs `tyhpdef/doctrine-doctrine-bundle-impl` (type files).
Require **this** name, not `tyhpdef/doctrine-doctrine-bundle-impl`.

See https://tyhplang.com.

## Maintain `doctrine/doctrine-bundle`? Ship the types yourself

If you are a Packagist maintainer of `doctrine/doctrine-bundle`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/doctrine-doctrine-bundle-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `doctrine/doctrine-bundle` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/doctrine-doctrine-bundle": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `doctrine/doctrine-bundle` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `doctrine/doctrine-bundle` with a real constraint,
   `"replace": { "tyhpdef/doctrine-doctrine-bundle": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `doctrine/doctrine-bundle` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/doctrine-doctrine-bundle` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->

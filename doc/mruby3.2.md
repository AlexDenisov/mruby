# User visible changes in `mruby3.2` from `mruby3.1`

# The language

- Now `a::B = c` should evaluate `a` then `c`.
- Anonymous arguments `*`, `**`, `&` can be passed for forwarding.
- Multi-precision integer is available now via `mruby-bigint` gem.

# mruby VM and bytecode

- `OP_ARYDUP` was renamed to `OP_ARYSPLAT`. The instruction name
  was changed but instruction number and basic behavior have not
  changed (except that `ARYDUP nil` makes `[]`).

# Tools

## `mruby`

- `-b` only specifies the script is the binary. The files loaded by `-r` are not affected by the option.
- `mruby` now loads complied binary if the suffix is `.mrb`.

## `mrbc`

- Add `--no-optimize` option to disable optimization.

# mrbgems

## mruby-class-ext

- Add `Class#subclasses` method.
- Add `Module#undefined_instance_methods` method.

## New bundled gems

- mruby-errno from [https://github.com/iij/mruby-errno.git]
- mruby-set from [https://github.com/yui-knk/mruby-set.git]
- mruby-dir from [https://github.com/iij/mruby-dir.git]

# CVEs

Following CVEs are fixed.

- [CVE-2022-0080](https://nvd.nist.gov/vuln/detail/CVE-2022-0080)
- [CVE-2022-0240](https://nvd.nist.gov/vuln/detail/CVE-2022-0240)
- [CVE-2022-0326](https://nvd.nist.gov/vuln/detail/CVE-2022-0326)
- [CVE-2022-0631](https://nvd.nist.gov/vuln/detail/CVE-2022-0631)
- [CVE-2022-0481](https://nvd.nist.gov/vuln/detail/CVE-2022-0481)
- [CVE-2022-0525](https://nvd.nist.gov/vuln/detail/CVE-2022-0525)
- [CVE-2022-0570](https://nvd.nist.gov/vuln/detail/CVE-2022-0570)
- [CVE-2022-0614](https://nvd.nist.gov/vuln/detail/CVE-2022-0614)
- [CVE-2022-0623](https://nvd.nist.gov/vuln/detail/CVE-2022-0623)
- [CVE-2022-0630](https://nvd.nist.gov/vuln/detail/CVE-2022-0630)
- [CVE-2022-0631](https://nvd.nist.gov/vuln/detail/CVE-2022-0631)
- [CVE-2022-0632](https://nvd.nist.gov/vuln/detail/CVE-2022-0632)
- [CVE-2022-0717](https://nvd.nist.gov/vuln/detail/CVE-2022-0717)
- [CVE-2022-0890](https://nvd.nist.gov/vuln/detail/CVE-2022-0890)
- [CVE-2022-1106](https://nvd.nist.gov/vuln/detail/CVE-2022-1106)
- [CVE-2022-1212](https://nvd.nist.gov/vuln/detail/CVE-2022-1212)
- [CVE-2022-1276](https://nvd.nist.gov/vuln/detail/CVE-2022-1276)
- [CVE-2022-1286](https://nvd.nist.gov/vuln/detail/CVE-2022-1286)
- [CVE-2022-1934](https://nvd.nist.gov/vuln/detail/CVE-2022-1934)

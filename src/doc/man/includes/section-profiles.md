## PROFILES

Profiles may be used to configure compiler options such as optimization levels
and debug settings. See [the reference](../reference/profiles.html) for more
details.

Profile selection depends on the target and crate being built. By default the
`dev` or `test` profiles are used. If the `--release` flag is given, then the
`release` or `bench` profiles are used.

Target | Default Profile | `--release` Profile
-------|-----------------|---------------------
lib, bin, example | `dev` | `release`
test, bench, or any target in "test" or "bench" mode | `test` | `bench`

Dependencies use the `dev`/`release` profiles.

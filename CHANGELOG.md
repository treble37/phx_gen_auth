# Changelog

## v0.5.0 (2020-09-03)

[Diff of generated code](https://github.com/aaronrenner/phx_gen_auth_output/compare/v0.4.0..v0.5.0)

### Enhancements

* Enabled same-site protection on remember me cookie. Thanks @mikl!
* Updated `UserAuth.require_athenticated_user/2` to remember query string
  parameters as part of the return_to path. Thanks @matthewlehner!
* Changed instances of "e-mail" to "email" to better match AP style guide.
  Thanks @zorn!
* Fixed arity in test context descriptions. Thanks @liamwhite!
* Fixed typos in generated documentation. Thanks @liamwhite!

## v0.4.0 (2020-06-19)

[Diff of generated code](https://github.com/aaronrenner/phx_gen_auth_output/compare/v0.3.0..v0.4.0)

### Enhancements

* Changed email form fields from `text_input` to `email_input`. Thanks @ream88!
* Renamed incorrect login/logout(nouns) to "log in"/"log out" (verbs).
* Replaced string-based route assertions with Routes-based assertions. Thanks @chvanikoff!
* `_user_menu.html` is now injected at the end of the `<nav>` tag, if possible.

## v0.3.0 (2020-05-26)

[Diff of generated code](https://github.com/aaronrenner/phx_gen_auth_output/compare/v0.2.0..v0.3.0)

### Enhancements

* Updated generated code be up to date through commit: [4664c3](https://github.com/dashbitco/mix_phx_gen_auth_demo/pull/1/commits/4664c376273af7100e31766ccf2d76bc7cf153e4). [[Diff](https://github.com/dashbitco/mix_phx_gen_auth_demo/compare/6ae63a...4664c3)]
* Upgraded phoenix requirement to `~> 1.5.2` to use undeprecated `MyApp.Endpoint.subscribe/1` function.
* Updated generator to be compatible with existing fixtures modules.
* Set `live_socket_id` on log in and disconnect on log out.
* Updated log out to succeed even if user is already logged out.
* Added index on user_tokens.user_id column
* Renamed several functions (see diff).

## v0.2.0 (2020-04-28)

[Diff of generated code](https://github.com/aaronrenner/phx_gen_auth_output/compare/v0.1.0..v0.2.0)

### Enhancements

* Updated generated code be up to date through commit: [6ae63a](https://github.com/dashbitco/mix_phx_gen_auth_demo/pull/1/commits/6ae63abbe5c2e2c37f47dea83da1b830374ebf18). [[Diff](https://github.com/dashbitco/mix_phx_gen_auth_demo/compare/ecc8eb...6ae63a)]
* Run `User.maybe_hash_password/1` in a `prepare_changes/1` hook instead of every time a changeset function is called. This decreases load on the server when a changeset function is being called multiple times like with a LiveView-based form.

## v0.1.0 (2020-04-24)

[Diff of generated code](https://github.com/aaronrenner/phx_gen_auth_output/compare/v0.1.0-rc.0..v0.1.0)

### Enhancements

* Upgraded phoenix dependency to `~> 1.5.0`.
* Updated generated code be up to date through commit: [ecc8eb](https://github.com/dashbitco/mix_phx_gen_auth_demo/pull/1/commits/ecc8eb596e52fb041c3518d58d13503e2e25e5d1). [[Diff](https://github.com/dashbitco/mix_phx_gen_auth_demo/compare/25d083...ecc8eb)]
* Print warnings instead of crashing on missing files.
* Raise error when app is generated with `--no-html`.
* Improve formatting of help messages.
* Added instructions for apps upgraded from Phoenix 1.4. Thanks @goofansu.

### Bug Fixes

* Log when `config/test.exs` is injected.


## v0.1.0-rc.0 (2020-04-17)

Initial release.

* Up to date with original PR through commit [25d083](https://github.com/dashbitco/mix_phx_gen_auth_demo/pull/1/commits/25d083d105a406ab3a1c10ee7ab1b2bb4af31345).

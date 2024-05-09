<a name="unreleased"></a>
## [Unreleased]

### Bug Fixes
- add enough to list of required applications
- typespecs for watchdog/1
- fix dialyzer error for systemd:set_status/1
- docs for `systemd_journal_h`
- Add Erlang 24 support ([#29](https://github.com/hauleth/erlang-systemd/issues/29))
- do not fail on invalid JOURNAL_STREAM content
- **journal:** use correct name for priority attribute
- **journal:** format message as Unicode-encoded binary
- **journal:** cleanup journal documentation
- **journal_h:** use proper check for socket existence
- **journal_h:** Dialyzer error
- **kmsg_formatter:** do not append log level on last newline
- **systemd_journal_h:** Support literal field values ([#25](https://github.com/hauleth/erlang-systemd/issues/25))
- **systemd_protocol:** keep empty values in encode_field/2 ([#27](https://github.com/hauleth/erlang-systemd/issues/27))

### Documentation
- correct the in-doc description of return value for watchdog/1
- fix typos
- add syntax highlighting on systemd example
- describe usage in Elixir projects
- fix typo equested -> requested
- imporve systemd.service example in the README
- **fds:** document new functions

### Features
- add warning log message if there is no readiness message sent
- send MAINPID message on socket start
- add functions to set custom status


<a name="0.5.0"></a>
## [0.5.0] - 2020-03-09
### Bug Fixes
- remove unneeded `handle_info/2` callbacks ([`fa77f8e`](https://github.com/hauleth/erlang-systemd/commit/fa77f8eb04d4cb46e9c8c42c60f9758276b7f0d9))

### Documentation
- update README ([`33cce22`](https://github.com/hauleth/erlang-systemd/commit/33cce223d7d629e86f7ccb8eb739b0c03238c655))
- fix typos in documentation ([`6a40613`](https://github.com/hauleth/erlang-systemd/commit/6a406132a090f029ae5e7174dd03f8674b14fc64))
- **systemd_kmsg_formatter:** add documentation about auto registration ([`4ecc76d`](https://github.com/hauleth/erlang-systemd/commit/4ecc76dbdd280b6942ccb9884cbb8195eb5e02c4))


<a name="0.4.0"></a>
## [0.4.0] - 2020-01-20
### Bug Fixes
- **systemd_stderr_formatter:** prefix all lines instead of only first one ([`1ccd500`](https://github.com/hauleth/erlang-systemd/commit/1ccd5002e7ab9e884a9947c948a46fd3ac93870e))

### Documentation
- add since documentation tags ([`abc7f28`](https://github.com/hauleth/erlang-systemd/commit/abc7f286390f855e9577c1488ea6d954ab8efc87))
- expand documentation on systemd and systemd_journal_formatter ([`f6e323c`](https://github.com/hauleth/erlang-systemd/commit/f6e323c2e764fe9d47dc0f1455af6e10755bc580))
- **systemd:** expand documentation of `unset_env/1` ([`630460e`](https://github.com/hauleth/erlang-systemd/commit/630460e40e0b0b8ff169547ef8737698f2a1db2e))
- **systemd_stderr_formatter:** hide implementation functions ([`f670d1f`](https://github.com/hauleth/erlang-systemd/commit/f670d1f2389a9a5a587f42be8ddc5c61b0cf3562))


<a name="0.3.3"></a>
## [0.3.3] - 2020-01-18
### Bug Fixes
- **systemd_journal_formatter:** check for empty data before building iolist ([`095088e`](https://github.com/hauleth/erlang-systemd/commit/095088eeed308869505bacc5a10af338e6f241b9))
- **systemd_journal_formatter:** again invalid format of multiline messages ([`b8f213a`](https://github.com/hauleth/erlang-systemd/commit/b8f213af5a51a06ca41badbb01669b7c0e64cd08))


<a name="0.3.2"></a>
## [0.3.2] - 2020-01-18
### Bug Fixes
- **systemd_journal_formatter:** improper multiline format ([`2c821e5`](https://github.com/hauleth/erlang-systemd/commit/2c821e5a9d3073fcf84ada2c7cff47f760e2f51e))


<a name="0.3.1"></a>
## [0.3.1] - 2020-01-18
### Bug Fixes
- **systemd_journal_formatter:** handling of unary report_cb return value ([`4a0577b`](https://github.com/hauleth/erlang-systemd/commit/4a0577b42db54bd67c54489b187e842c4638d423))


<a name="0.3.0"></a>
## [0.3.0] - 2020-01-18
### Bug Fixes
- move environment variables extraction to supervisor ([`d889d67`](https://github.com/hauleth/erlang-systemd/commit/d889d6739c6da10fb5d9efb0b7518ba0144b8721))
- **systemd_watchdog:** convert timeout from microseconds to milliseconds ([`fec0e26`](https://github.com/hauleth/erlang-systemd/commit/fec0e26f2bfe964df0c8eb96b1f1f0723add84b5))
- **systemd_watchdog:** use send_after instead of timeouts ([`c85c095`](https://github.com/hauleth/erlang-systemd/commit/c85c09558009bfca9dbb1b4286823539451ea83b))
- **systemd_watchdog:** initial timeout was off ([`d8839b7`](https://github.com/hauleth/erlang-systemd/commit/d8839b7d126a717a2d98bdaeec44b48d48c6b54a))

### Documentation
- add informations about journal loggers ([`20718cc`](https://github.com/hauleth/erlang-systemd/commit/20718cc553270783b476bd9ee08b338e038c4fc3))
- **README:** extend example with more correct systemd service ([`ab3c3fa`](https://github.com/hauleth/erlang-systemd/commit/ab3c3fa85899b9a797197b6d24b55099e0fb71a9))
- **systemd_formatter:** document usage ([`5c3e3ba`](https://github.com/hauleth/erlang-systemd/commit/5c3e3bab79ac4e4bbef558be89192c552ec3ee65))
- **systemd_journal_h:** add warnings about required formatter ([`3e09c7c`](https://github.com/hauleth/erlang-systemd/commit/3e09c7cac642233900bb8e52a9d43888ff5b6f8e))
- **systemd_stderr_formatter:** fix missing tag ([`31f1b60`](https://github.com/hauleth/erlang-systemd/commit/31f1b60ed023f665b16d51a98efce1403db960cf))


<a name="0.1.2"></a>
## [0.1.2] - 2020-01-15
### Bug Fixes
- **systemd_watchdog:** convert time unit from micro to milliseconds ([`2a40a6e`](https://github.com/hauleth/erlang-systemd/commit/2a40a6e30fd5052bbf59ad3524230211e2993693))


<a name="0.2.0"></a>
## [0.2.0] - 2020-01-15
### Bug Fixes
- **systemd_watchdog:** convert timeout from microseconds to milliseconds ([`fec0e26`](https://github.com/hauleth/erlang-systemd/commit/fec0e26f2bfe964df0c8eb96b1f1f0723add84b5))
- **systemd_watchdog:** use send_after instead of timeouts ([`c85c095`](https://github.com/hauleth/erlang-systemd/commit/c85c09558009bfca9dbb1b4286823539451ea83b))
- **systemd_watchdog:** initial timeout was off ([`d8839b7`](https://github.com/hauleth/erlang-systemd/commit/d8839b7d126a717a2d98bdaeec44b48d48c6b54a))


<a name="0.1.1"></a>
## [0.1.1] - 2020-01-15
### Bug Fixes
- **systemd_app:** remove start_phase ([`a9e5905`](https://github.com/hauleth/erlang-systemd/commit/a9e5905f2e00dcb76ae8243d9415e15bb1e3f3ed))
- **systemd_socket:** unused variable ([`1d51b2e`](https://github.com/hauleth/erlang-systemd/commit/1d51b2eeac8a7d13836808a8f71b71480b32541c))
- **systemd_watchdog:** one missed direct call to socket ([`0fce8eb`](https://github.com/hauleth/erlang-systemd/commit/0fce8eb1f3880d10d0c88f1356a7bc894ffeae8d))


<a name="0.1.0"></a>
## 0.1.0 - 2020-01-15

[Unreleased]: https://github.com/hauleth/erlang-systemd/compare/0.5.0...HEAD
[0.5.0]: https://github.com/hauleth/erlang-systemd/compare/0.4.0...0.5.0
[0.4.0]: https://github.com/hauleth/erlang-systemd/compare/0.3.3...0.4.0
[0.3.3]: https://github.com/hauleth/erlang-systemd/compare/0.3.2...0.3.3
[0.3.2]: https://github.com/hauleth/erlang-systemd/compare/0.3.1...0.3.2
[0.3.1]: https://github.com/hauleth/erlang-systemd/compare/0.3.0...0.3.1
[0.3.0]: https://github.com/hauleth/erlang-systemd/compare/0.1.2...0.3.0
[0.1.2]: https://github.com/hauleth/erlang-systemd/compare/0.2.0...0.1.2
[0.2.0]: https://github.com/hauleth/erlang-systemd/compare/0.1.1...0.2.0
[0.1.1]: https://github.com/hauleth/erlang-systemd/compare/0.1.0...0.1.1

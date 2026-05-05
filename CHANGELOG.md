# Changelog

## [2.0.0](https://github.com/yonasBSD/SpoofDPI/compare/v1.5.0...v2.0.0) (2026-05-05)


### ⚠ BREAKING CHANGES

* The --allow and --ignore flags have been removed. Please use --policy="i:domain.com"` or `--policy="x:domain.com" instead.

### Features

* add `disorder` option ([#332](https://github.com/yonasBSD/SpoofDPI/issues/332)) ([15cd32e](https://github.com/yonasBSD/SpoofDPI/commit/15cd32e0346ddc7d5f88ef0b8d2fa25bc22053ce))
* add auto-policy option ([5e0ad7e](https://github.com/yonasBSD/SpoofDPI/commit/5e0ad7e32d28979f67b5a71f6886e724746dc63d))
* add IPv6 support ([#161](https://github.com/yonasBSD/SpoofDPI/issues/161)) ([15163ca](https://github.com/yonasBSD/SpoofDPI/commit/15163ca5fe6ad0fe383773ce7def4ece688d6535))
* **config:** eager-resolve policy overrides at load time ([fc4cafd](https://github.com/yonasBSD/SpoofDPI/commit/fc4cafd3c5ae734a44d4a84cec0a35e314b9f6fd))
* **config:** pretty-print rules in trace logs via per-type MarshalJSON ([c16a9c5](https://github.com/yonasBSD/SpoofDPI/commit/c16a9c5be32539ac0b222481ae4c9f6fc0f9fed1))
* **config:** summarize match domains/addrs and segments as "N items" ([0908cd5](https://github.com/yonasBSD/SpoofDPI/commit/0908cd50c1c950c174d0a67034a154f1b81164bd))
* DNS. Add the ability to disable version 6 address resolution ([#240](https://github.com/yonasBSD/SpoofDPI/issues/240)) ([abd7441](https://github.com/yonasBSD/SpoofDPI/commit/abd7441d0a0373ee44481652f6133ac69e3c9963))
* enhance proxy/server.go and refactor ([a40e94b](https://github.com/yonasBSD/SpoofDPI/commit/a40e94bf4438032902f1f042fc23978eada87186))
* **hop:** add bpf filter to hop tracker ([6d23806](https://github.com/yonasBSD/SpoofDPI/commit/6d2380613d1cd47d826ea3d01edfe46ad7be0c79))
* improve rule configuration system ([#341](https://github.com/yonasBSD/SpoofDPI/issues/341)) ([6392bf4](https://github.com/yonasBSD/SpoofDPI/commit/6392bf4b509597ca0af5a616074ffdeb2e118fea))
* ipv6 joins the ride. ([714daea](https://github.com/yonasBSD/SpoofDPI/commit/714daeab99972e93fc738364f23f06360bbff3eb))
* merge --allow/--ignore flags into --policy ([#307](https://github.com/yonasBSD/SpoofDPI/issues/307)) ([a5159d5](https://github.com/yonasBSD/SpoofDPI/commit/a5159d5efe1e8db555cf2d30d4fb77e99cf971bc))
* move doh to internal ([dbe7f32](https://github.com/yonasBSD/SpoofDPI/commit/dbe7f32a1fdba864dd164c3444dcfed714e079b3))
* rename --patern argument to --allow and add --ignore argument ([a3e2985](https://github.com/yonasBSD/SpoofDPI/commit/a3e29858fac0d1026980975173be9d44e97d81ae))
* **server:** register UDP destinations with sniffer for fake-packet TTL ([4c2fb3b](https://github.com/yonasBSD/SpoofDPI/commit/4c2fb3b0e390d8672ac2d338cbf5fe28a5c36362))
* support socks5 and tun modes ([#364](https://github.com/yonasBSD/SpoofDPI/issues/364)) ([da3268d](https://github.com/yonasBSD/SpoofDPI/commit/da3268d51a765d7f8fbf0588de308cde7d83f7ac))
* support toml config file ([#300](https://github.com/yonasBSD/SpoofDPI/issues/300)) ([171b64f](https://github.com/yonasBSD/SpoofDPI/commit/171b64fd48fc509b1c1ff9279ffdfe680b3d193b))
* support TUI mode ([#378](https://github.com/yonasBSD/SpoofDPI/issues/378)) ([b0c489b](https://github.com/yonasBSD/SpoofDPI/commit/b0c489bfebabac6adf2e0028ed9594de150cb22e))
* tidy up unnecessary logs and add log-level flag ([#301](https://github.com/yonasBSD/SpoofDPI/issues/301)) ([04ee83d](https://github.com/yonasBSD/SpoofDPI/commit/04ee83d41e510f851c4afd9546a81190d04d639b))


### Bug Fixes

* [#365](https://github.com/yonasBSD/SpoofDPI/issues/365) ([#367](https://github.com/yonasBSD/SpoofDPI/issues/367)) ([48142a4](https://github.com/yonasBSD/SpoofDPI/commit/48142a4efed40705a5bc3a60ec1705a67f9b8a40))
* [#46](https://github.com/yonasBSD/SpoofDPI/issues/46) ([363f022](https://github.com/yonasBSD/SpoofDPI/commit/363f022c91773acd62f306ba9bae5bfae4913c2a))
* 21 ([d15a24a](https://github.com/yonasBSD/SpoofDPI/commit/d15a24a2a118dadd7abbd730f741e78a0f3043f5))
* add new line after printing version ([#329](https://github.com/yonasBSD/SpoofDPI/issues/329)) ([3f16fd2](https://github.com/yonasBSD/SpoofDPI/commit/3f16fd29ab387dd0b873a9461c31288709138199))
* check TLS if payload with invalid length ([#172](https://github.com/yonasBSD/SpoofDPI/issues/172)) ([73e5fec](https://github.com/yonasBSD/SpoofDPI/commit/73e5fec093885e601926b61fc4fe2cd5b437243b))
* client hello ([852b789](https://github.com/yonasBSD/SpoofDPI/commit/852b789ac3f5b52288a2136102dea6408e2a55b7))
* client hello ([6b0547b](https://github.com/yonasBSD/SpoofDPI/commit/6b0547b4310b90cb1c31fc30250b380ec6245308))
* client hello ([1f7fe64](https://github.com/yonasBSD/SpoofDPI/commit/1f7fe642d58dd53ea05ffaecdf8db7ad6702a2f9))
* client hello ([4c0f5ca](https://github.com/yonasBSD/SpoofDPI/commit/4c0f5ca6c8c6313382ff4655f8bfdea890be8796))
* condition for shouldExploit ([#306](https://github.com/yonasBSD/SpoofDPI/issues/306)) ([874e42c](https://github.com/yonasBSD/SpoofDPI/commit/874e42c3c3312bcc4d1deccb88da3da462a46660))
* **config:** reset rule https.skip when not explicitly set ([6715b21](https://github.com/yonasBSD/SpoofDPI/commit/6715b21983a732ea1b1734529f64fa1ccfa4ae74))
* Fix the problem not being able to run the binaries ([ea90ea8](https://github.com/yonasBSD/SpoofDPI/commit/ea90ea8eb1062c48dbb6a458ff57083aa9f4bb0e))
* get ctx logger on new request ([#198](https://github.com/yonasBSD/SpoofDPI/issues/198)) ([2aea4a7](https://github.com/yonasBSD/SpoofDPI/commit/2aea4a7a51e1709e759211507f18bb65392cb4c2))
* help text for --ignore argument ([c502bfd](https://github.com/yonasBSD/SpoofDPI/commit/c502bfd76750047ca4bd78a8fa95cdab497be3d3))
* IPv6 support ([#177](https://github.com/yonasBSD/SpoofDPI/issues/177)) ([87161e0](https://github.com/yonasBSD/SpoofDPI/commit/87161e053899cafa8b99a5caa956551ab935f05b))
* **main:** return early when createServer fails to avoid nil-deref on ListenAndServe ([#382](https://github.com/yonasBSD/SpoofDPI/issues/382)) ([2aa53d0](https://github.com/yonasBSD/SpoofDPI/commit/2aa53d091bd20b31f14659fd0a3a8cf216175544))
* make doh truly singleton ([e9de332](https://github.com/yonasBSD/SpoofDPI/commit/e9de332163f212a8d5fc513cbcc4995ad314e663))
* **matcher:** resolve duplicate-domain rules by priority ([894b6ae](https://github.com/yonasBSD/SpoofDPI/commit/894b6ae28acddaec89e99d8ba0f63cb56d00cc43))
* **matcher:** tighten conflict error format to avoid escaped quotes ([b5e82df](https://github.com/yonasBSD/SpoofDPI/commit/b5e82dfa80467c1e2a42e12b8d092e7a5d808a30))
* mistyped receiver for dns/resolver/general.go ([59a6d7b](https://github.com/yonasBSD/SpoofDPI/commit/59a6d7b376fb88696dfff0525654a933720830af))
* nil pointer deref ([fa2cfc4](https://github.com/yonasBSD/SpoofDPI/commit/fa2cfc4c8c7f23d720124fa2899b1b17a7b4bb43))
* nil pointer for StringArray ([ab4d681](https://github.com/yonasBSD/SpoofDPI/commit/ab4d6819c7f8f82fb3f58cbc2ec2ff34af853948))
* packet processing for http request ([#230](https://github.com/yonasBSD/SpoofDPI/issues/230)) ([79d2557](https://github.com/yonasBSD/SpoofDPI/commit/79d255719ed75688ad3d27379c3e15591db3b2eb))
* **packet:** re-add missing ethtLayer ([7de4e44](https://github.com/yonasBSD/SpoofDPI/commit/7de4e44330cba92f50094a5da5525aa17841c420))
* **packet:** resolve import cycle ([f9518a6](https://github.com/yonasBSD/SpoofDPI/commit/f9518a696f0eee7a8f633c4d42587dbd7118d8e1))
* **packet:** return wrapped DefaultPcapHandle instead of pcap.Handle ([32fcd69](https://github.com/yonasBSD/SpoofDPI/commit/32fcd69a47c89c5b379a8874db587828952e581b))
* producing timeout error in case with no timeout errors ([#180](https://github.com/yonasBSD/SpoofDPI/issues/180)) ([d97d4e4](https://github.com/yonasBSD/SpoofDPI/commit/d97d4e483ce2806ff988630cd68ebe46583d5771))
* **proxy:** check if hopTracker is nil before running RegisterUntracked() ([#325](https://github.com/yonasBSD/SpoofDPI/issues/325)) ([fd659be](https://github.com/yonasBSD/SpoofDPI/commit/fd659bef867941325893127e23a65f4e6a1ed6eb))
* **proxy:** go routine leak for tunnel function ([#311](https://github.com/yonasBSD/SpoofDPI/issues/311)) ([76de361](https://github.com/yonasBSD/SpoofDPI/commit/76de361465435e90ac0462e04491b22bea743d1f))
* re-add handling leading https and trailing /dns-query ([84ad728](https://github.com/yonasBSD/SpoofDPI/commit/84ad7288eac69dc81175f3dce4ec34a1c411dbd1))
* re-implement cancellation context ([c93ddd6](https://github.com/yonasBSD/SpoofDPI/commit/c93ddd67e0ee4b789f5d87baedf5cc3109e4dc38))
* remove automatic retry when doh fails ([c8c18a4](https://github.com/yonasBSD/SpoofDPI/commit/c8c18a46510135cddd0189c9c2fd21a9c250afe4))
* remove unused imports ([2e45975](https://github.com/yonasBSD/SpoofDPI/commit/2e45975ea9c129aff5cd12f6532b19033f47cbe3))
* termination instruction message ([1f26fbd](https://github.com/yonasBSD/SpoofDPI/commit/1f26fbd2e31abdc5bcfe266ce01fbcf213acd753))
* **tui:** keep TUI alive on startup errors so user can read them ([956eb9c](https://github.com/yonasBSD/SpoofDPI/commit/956eb9c5c6409d2bb342bc8fad3383ba8f4a23d4))
* **tui:** preserve log line color across wrapped continuations ([22bac0b](https://github.com/yonasBSD/SpoofDPI/commit/22bac0b922d82d81ea7e6bf449117d23fcc14be6))
* **tui:** switch log wrap from word-wrap to hardwrap ([041cf52](https://github.com/yonasBSD/SpoofDPI/commit/041cf52cb20a3845d1af6e61afc48f5853d5bb4e))
* **tui:** wrap log lines to viewport width ([2b76cde](https://github.com/yonasBSD/SpoofDPI/commit/2b76cde984977a92cdab22dc96f5d209183cc556))
* unmatched types error for system.SetProxy() ([#295](https://github.com/yonasBSD/SpoofDPI/issues/295)) ([dfa240a](https://github.com/yonasBSD/SpoofDPI/commit/dfa240a665c96bd43eea637581d40772fa1c0592))
* update accumulator for total bytes written ([341d476](https://github.com/yonasBSD/SpoofDPI/commit/341d47622cf1afd2133eeb1fb86f2213c10c79af))
* use fmt.Println to print version information ([#326](https://github.com/yonasBSD/SpoofDPI/issues/326)) ([3f5e1eb](https://github.com/yonasBSD/SpoofDPI/commit/3f5e1eb7447a8da6f93b485f6fa35e1a7c5f13b0))


### Performance Improvements

* remove loop ([dbee496](https://github.com/yonasBSD/SpoofDPI/commit/dbee4964f8eb655b9e54e0fb5ba6ac197ab7b7f8))
* remove loop ([8843892](https://github.com/yonasBSD/SpoofDPI/commit/884389256db6afb2e9ee2a493ef441b80832559e))
* reuse allocated buffer ([c76e21c](https://github.com/yonasBSD/SpoofDPI/commit/c76e21cec0a8cfe370577c99dfe193e854f16969))
* reuse allocated buffer. add config parameter ([10d1ee4](https://github.com/yonasBSD/SpoofDPI/commit/10d1ee4860a8a7b84f1d38e398df9da553518d2c))
* reuse allocated buffer. add config parameter ([6d87e67](https://github.com/yonasBSD/SpoofDPI/commit/6d87e679ad61b0266cf112222db73b37b3453655))
* reuse allocated buffer. add config parameter ([7bf3f9e](https://github.com/yonasBSD/SpoofDPI/commit/7bf3f9e4e5703a10bfedc05e38f1286d710695bc))

## [1.5.0](https://github.com/xvzc/spoofdpi/compare/v1.4.1...v1.5.0) (2026-05-04)


### Features

* **config:** eager-resolve policy overrides at load time ([fc4cafd](https://github.com/xvzc/spoofdpi/commit/fc4cafd3c5ae734a44d4a84cec0a35e314b9f6fd))
* **config:** pretty-print rules in trace logs via per-type MarshalJSON ([c16a9c5](https://github.com/xvzc/spoofdpi/commit/c16a9c5be32539ac0b222481ae4c9f6fc0f9fed1))
* **config:** summarize match domains/addrs and segments as "N items" ([0908cd5](https://github.com/xvzc/spoofdpi/commit/0908cd50c1c950c174d0a67034a154f1b81164bd))
* **server:** register UDP destinations with sniffer for fake-packet TTL ([4c2fb3b](https://github.com/xvzc/spoofdpi/commit/4c2fb3b0e390d8672ac2d338cbf5fe28a5c36362))


### Bug Fixes

* **config:** reset rule https.skip when not explicitly set ([6715b21](https://github.com/xvzc/spoofdpi/commit/6715b21983a732ea1b1734529f64fa1ccfa4ae74))
* **matcher:** resolve duplicate-domain rules by priority ([894b6ae](https://github.com/xvzc/spoofdpi/commit/894b6ae28acddaec89e99d8ba0f63cb56d00cc43))
* **matcher:** tighten conflict error format to avoid escaped quotes ([b5e82df](https://github.com/xvzc/spoofdpi/commit/b5e82dfa80467c1e2a42e12b8d092e7a5d808a30))
* **tui:** keep TUI alive on startup errors so user can read them ([956eb9c](https://github.com/xvzc/spoofdpi/commit/956eb9c5c6409d2bb342bc8fad3383ba8f4a23d4))
* **tui:** preserve log line color across wrapped continuations ([22bac0b](https://github.com/xvzc/spoofdpi/commit/22bac0b922d82d81ea7e6bf449117d23fcc14be6))
* **tui:** switch log wrap from word-wrap to hardwrap ([041cf52](https://github.com/xvzc/spoofdpi/commit/041cf52cb20a3845d1af6e61afc48f5853d5bb4e))
* **tui:** wrap log lines to viewport width ([2b76cde](https://github.com/xvzc/spoofdpi/commit/2b76cde984977a92cdab22dc96f5d209183cc556))

## [1.4.1](https://github.com/xvzc/spoofdpi/compare/v1.4.0...v1.4.1) (2026-05-03)


### Bug Fixes

* **main:** return early when createServer fails to avoid nil-deref on ListenAndServe ([#382](https://github.com/xvzc/spoofdpi/issues/382)) ([2aa53d0](https://github.com/xvzc/spoofdpi/commit/2aa53d091bd20b31f14659fd0a3a8cf216175544))

## [1.4.0](https://github.com/xvzc/spoofdpi/compare/v1.3.1...v1.4.0) (2026-04-29)


### Features

* support TUI mode ([#378](https://github.com/xvzc/spoofdpi/issues/378)) ([b0c489b](https://github.com/xvzc/spoofdpi/commit/b0c489bfebabac6adf2e0028ed9594de150cb22e))

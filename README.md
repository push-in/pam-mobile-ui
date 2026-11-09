<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset=".github/assets/banner-dark.svg">
  <img src=".github/assets/banner-light.svg" width="880" alt="pam-mobile-ui: Compatibility package. New projects require pushinbr/pam-native-ui.">
</picture>

**Compatibility package: use [PAM Native UI](https://github.com/push-in/pam-native-ui) (`pushinbr/pam-native-ui`).**<br>
This name stays installable so older Composer projects keep resolving. Do not use it in new applications.

[![Packagist](https://img.shields.io/packagist/v/pushinbr/pam-mobile-ui?label=packagist&color=f53003)](https://packagist.org/packages/pushinbr/pam-mobile-ui)
![PHP 8.5](https://img.shields.io/badge/php-8.5-777bb4)
[![License](https://img.shields.io/github/license/push-in/pam-mobile-ui?color=1f6feb)](LICENSE)
[![Replacement](https://img.shields.io/badge/replacement-pushinbr/pam--native--ui-f53003)](https://packagist.org/packages/pushinbr/pam-native-ui)
![Status](https://img.shields.io/badge/status-migration%20only-e3a008)

[Use instead](#install) · [Migrate](#migrate) · [Support policy](#support-policy) · [PAM Native UI](https://github.com/push-in/pam-native-ui)

</div>

<a id="install"></a>
## <picture><img src=".github/assets/icons/terminal.svg" width="22" height="22" alt=""></picture> Install

Inside a PAM project, require the maintained package instead:

```sh
pam composer require pushinbr/pam-native-ui
```

[PAM Native UI](https://github.com/push-in/pam-native-ui) has the active documentation, API examples, releases, issue tracker and production guidance. Requiring this package installs `pushinbr/pam-native-ui` `^0.5` (see `composer.json`), while the replacement's current release is v1.0.8: require it directly to follow its current major.

<a id="migrate"></a>
## <picture><img src=".github/assets/icons/terminal.svg" width="22" height="22" alt=""></picture> Migrate an existing project

Commit your current `composer.json` and `composer.lock`, then run:

```sh
pam composer remove pushinbr/pam-mobile-ui
pam composer require pushinbr/pam-native-ui
pam doctor
```

Run the application test suite before committing the new lockfile. Composer may continue to resolve this package transitively during a staged migration; application code should target the replacement package directly.

<a id="why"></a>
## <picture><img src=".github/assets/icons/sparkle.svg" width="22" height="22" alt=""></picture> Why the name changed

The ecosystem uses Native consistently for Android and iOS products; the old Mobile name is retained only so existing lockfiles keep resolving.

<a id="support-policy"></a>
## <picture><img src=".github/assets/icons/shield.svg" width="22" height="22" alt=""></picture> Support policy

- No new features are added here.
- Security or resolution fixes may be published only to preserve migration safety.
- New documentation and issues belong to [PAM Native UI](https://github.com/push-in/pam-native-ui).
- The package is marked abandoned on Packagist in favor of `pushinbr/pam-native-ui`.

This explicit compatibility repository is intentional: old installs remain understandable without making the current PAM ecosystem ambiguous.

<a id="pam-ecosystem"></a>
## <picture><img src=".github/assets/icons/plug.svg" width="22" height="22" alt=""></picture> Part of the PAM ecosystem

<p align="center"><picture>
  <source media="(prefers-color-scheme: dark)" srcset=".github/assets/pam-wordmark-dark.svg">
  <img src=".github/assets/pam-wordmark-light.svg" height="56" alt="PAM">
</picture></p>

PAM runs PHP natively on servers, desktops and phones. This repository only keeps an old package name resolvable.

| [**PAM**](https://github.com/push-in/pam) | [**PAM Desktop**](https://github.com/push-in/pam-desktop) | [**PAM Native**](https://github.com/push-in/pam-native) | [**Ecosystem**](https://github.com/push-in/pam#ecosystem) |
| --- | --- | --- | --- |
| the runtime and CLI | native desktop apps in PHP | native Android and iOS apps in PHP | every official package and plugin |

<sub>Docs: [push-in.github.io/pam-docs](https://push-in.github.io/pam-docs/introduction/) · [Issues](https://github.com/push-in/pam-mobile-ui/issues)</sub>

<p align="center"><sub><a href="LICENSE">Apache-2.0</a> · Made in Brazil by Pushin</sub></p>

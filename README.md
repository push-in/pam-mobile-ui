# pushinbr/pam-mobile-ui

This name is retained only for migration compatibility. The product is now
[`pushinbr/pam-native-ui`](https://packagist.org/packages/pushinbr/pam-native-ui).

## Start here

```bash
curl -fsSL https://push-in.github.io/pam/install.sh | sh
pam doctor
pam composer remove pushinbr/pam-mobile-ui
pam composer require pushinbr/pam-native-ui
```

Existing projects may keep resolving this package temporarily because it
depends on the replacement. New code must require `pushinbr/pam-native-ui` directly.

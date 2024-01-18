# tpivault
[Two Person Integrity](https://en.m.wikipedia.org/wiki/Two-person_rule) enabled Vault for sensitive secrets, like AWS root MFA QR codes to avoid the safe-in-a-safe madness.

A web app that integrates at least with Microsoft Entra, to provides access to secrets via SSO enabled MFA authentication, only if two persons of proper membership authenticates successfully, within something like 30 minuttes.

Maybe identity providers like GitHub or Apple could be added.

Maybe even build a [virtual authenticator](https://docs.rs/passkey/latest/passkey/) app, that provides the required TOTP secret, instead of a revealing the MFA QR.

Maybe use something like [Shamir's secret sharing](https://en.m.wikipedia.org/wiki/Shamir%27s_secret_sharing) for the vault.

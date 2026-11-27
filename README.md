# Fundy — Releases

Public release binaries for **Fundy**, the DSDA BSV wallet and browser.

## What is Fundy?

Fundy is a self-custodial BSV wallet with a built-in browser, arcade,
and Web3 capabilities. It is built by DSDA (ds-da.ca) on top of the
[bsv-browser](https://github.com/bsv-blockchain/bsv-browser) project and the
`@bsv/expo-wallet-toolbox`.

- **Website:** [ds-da.ca/pocket](https://ds-da.ca/pocket)
- **Source code:** [onebender137/pocket-wallet](https://github.com/onebender137/pocket-wallet) (private)

## Downloading the APK

The latest release is always available at:

```
https://github.com/onebender137/fundy-releases/releases/latest/download/fundy.apk
```

To install:
1. Download `fundy.apk`.
2. Transfer it to your Android device (or open the link on the device).
3. Enable "Install unknown apps" for your browser/file manager.
4. Open the APK and follow the install prompts.

## Signing certificate

All releases are signed with the DSDA release key. Verify the certificate
fingerprint before installing:

```
SHA-256: D2:D0:C1:3D:D1:C8:1B:A4:29:2A:31:F4:46:E9:2D:69:24:17:50:2E:CB:A5:14:15:52:AA:87:35:53:66:9B:C7
Subject: CN=Pocket Wallet, OU=DSDA, O=DSDA, C=CA
```

You can verify a downloaded APK with:

```
apksigner verify --print-certs fundy.apk
```

The `Signer #1 certificate SHA-256 digest` should match the fingerprint above
(colons removed).

## Package

- **Package name:** `ca.dsda.wallet`
- **Architecture:** arm64-v8a only
- **Minimum SDK:** 24 (Android 7.0)
- **Target SDK:** 36 (Android 16)

## License

Fundy is distributed under the **Apache License 2.0**. See
[`LICENSE`](LICENSE) and [`NOTICE`](NOTICE). Both files ship with every binary
release, as required by Apache-2.0.

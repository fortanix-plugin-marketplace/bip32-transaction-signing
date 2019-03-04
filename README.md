# Hierarchical Deterministic (HD) wallets Plugin
This plugin allows you to derive BIP32 child key pair (xprv, xpub) from BIP32 master key
## Initial setup
* import BIP32 master key in SDKMS as secrete object in raw byte format

**Example BIP32 Master Key:** xprv9s21ZrQH143K2yLSxbXemfny4nZroqhpiXEQ1MYx8vo2k7HRXypsWesNr7GkWTuU9CeaW7QeR38NjjaSfZBAAZVkVEpXwEkxLLXP2q1iFUd

## Plugin input and output for transaction signing for BIP32
Plugin takes master key-id, derivation path and message as json input and return signature as response

**Example: Input**
```
{
	"masterKeyId": "fbd70d51-9719-4da8-8f0f-1d304b78df44",
	"path": "m/2",
	"message" :"Fortanix"
}
```
**Example: Output**
```
{
	"signature": "MEUCICliuKqEHJzPXOBFsiYhHribAi8IZIbmCYx4bMZQ6KyuAiEA0khD8lYJEWxI5cwtPbOGRPFSaNv07omvpiOqYqW6tNM="
}
```

# License

This project is primarily distributed under the terms of the Apache License, Version 2.0 (the "License"), see [LICENSE](./LICENSE) for details.

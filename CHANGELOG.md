# Changelog

## 0.3.1 — 19 November 2026
Compatibility: Bagisto 2.5.1 and above, PHP 8.4, Laravel 13.

Corrected browser/server wallet validation, expanded encrypted order snapshots, kept unsigned carts active, made checkout creation POST-only, added maintenance middleware, removed the internal controller dependency, and added Intent Contract/Proxy/Repository support. Added stock/cart revalidation and regression coverage. Base USDC is enabled; BNB remains Coming soon and disabled.

### Distribution layout revision — 20 November 2026
Repacked the same reviewed version using `packages/XPay/Bagisto/`, with root README and changelog. Migrations now live in `src/Database/Migrations/`. Intent model registration moved to a dedicated `ModuleServiceProvider` extending Bagisto's `CoreModuleServiceProvider`, registered by `XPayServiceProvider`. The namespace and Composer path installation remain unchanged. No payment amounts, chain behavior or settlement implementation changed.

## 0.3.0 — 18 November 2026
Compatibility: Bagisto 2.5.1 and above, PHP 8.4, Laravel 13.

Moved credentials to per-channel admin settings, introduced simulated test mode and atomic cache locks, required USD base/checkout currencies, created orders only after payment verification, and added scheduled reconciliation, expiry, translations and sanitized logging.

## 0.2.2 — 17 November 2026
Initial Base USDC review release. Tested on Bagisto 2.5.1, PHP 8.4 and MySQL. Superseded by 0.3.1; not compatible with Bagisto 2.5.0 because its checkout API requires 2.5.1. Historical owner-approved 0.01 USDC payment evidence applies to this release only.

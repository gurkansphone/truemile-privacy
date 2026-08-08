# TrueMile EV — Privacy Policy

**Effective date: August 7, 2026**

TrueMile EV ("the app") is built and operated by Gate Engineering LLC. This policy describes
exactly what data the app handles, where it goes, and how you can delete it. It is written to be
read, not skimmed — there is nothing hidden in it.

## The short version

- Your data is used to run **your own** trip and charging history. Nothing else.
- **No ads. No sale of data. No third-party analytics or tracking SDKs.**
- Your data lives in the app's own private cloud database, keyed to your account.
- Deleting your account in the app deletes your cloud data.

## What the app collects

| Data | Why |
|---|---|
| **Email address** | Account sign-in (authentication only). |
| **Vehicle VIN and vehicle specs** (make, model, year, battery details; optional door-jamb label photos you choose to capture) | Identifies your vehicle so your trips, charges, and efficiency stats are computed for the right car. |
| **Trip GPS routes** (location breadcrumbs while driving, odometer, speed, energy use) | Automatic trip logging and per-trip maps — the core feature of the app. |
| **Charge sessions** (charger location, energy delivered, price you enter, timestamps) | Your charging history, cost tracking, and charging-curve analytics. |
| **Crash reports** (stack trace, app version, device model, a random install identifier) | Fixing bugs. The identifier is random — it is not your email, account, or advertising ID. |

## Where it lives

Your data is stored in the app's own database project (hosted on Supabase), in a private account
scoped to your sign-in. It is not shared with, rented to, or sold to anyone. Access is restricted
by row-level security to your own account.

Some data also lives **only on your device**: app settings, diagnostic logs (off by default,
opt-in, and only ever leave the phone if you personally share the file), and cached map data.

## Background location

The app asks for background ("Allow all the time") location because **automatic trip logging is
the core feature**: it detects when you start driving and records the route without you opening
the app. Location is recorded for your own trip history. It is not used for advertising, profiling,
or location sharing of any kind. You can decline background location; trip logging then only works
while the app is open.

## Third-party services the app talks to

The app queries a small number of services to do its job. Each receives only what the feature
needs, never your identity:

- **Charger directories** (NREL / Open Charge Map): the map region you are viewing, to list
  nearby chargers.
- **Routing** (OSRM): route coordinates, to draw and time your planned route.
- **Community charger prices** (optional, on by default, can be turned off in Settings): when you
  log a paid public charge, the station's location, price, and speed can be contributed to a shared
  community dataset under a **random anonymous identifier** — never your email, account, or VIN.
  Home charging is **never** contributed.

None of these are analytics or advertising services.

## What the app does NOT do

- No advertising, ad SDKs, or ad identifiers.
- No sale or sharing of personal data with data brokers.
- No third-party analytics (no Google Analytics, Firebase Analytics, Mixpanel, etc.).
- No reading of contacts, messages, photos (other than vehicle photos you take in-app), or any
  data unrelated to driving and charging.

## Retention and deletion

- Your cloud data is kept for as long as you keep your account.
- **Settings → Delete account** permanently removes your personal cloud data — your identity,
  email, trips, routes, GPS locations, home coordinates, charging locations, prices and costs,
  notes, settings, and generated reports.
- Uninstalling the app removes all local data from the device.
- Crash reports and anonymous community price contributions are retained only in aggregate and are
  not linked to a deleted account.

**The vehicle's health record stays with the vehicle.** When you delete your account, an
anonymized battery and condition history is retained, keyed only to the vehicle's VIN — like a
service book that follows the car to its next owner. It contains vehicle facts only:

- The vehicle's identity card: make, model, year, battery pack size, and the door-jamb sticker
  specifications (manufacture date, weight ratings, tire and rim sizes, cold tire pressures).
- Charging sessions at day-level dates: odometer, battery percentage before/after, energy added,
  duration, fast-vs-slow charging, outside temperature, and the charging-power curve.
- Battery state-of-health readings by date.
- Diagnostic trouble codes read from the vehicle, and tire fitment records.

It can never contain your name, email, or any account link; any location; any price, cost, or
payment information; any trip or route; or any free-text notes — the retained record has no
fields for them. If you also want this vehicle history removed, email us with the VIN before
deleting your account and we will exclude it.

## Children

The app is a vehicle telemetry tool and is not directed at children under 13.

## Changes

If this policy changes, the updated version will be posted at this URL with a new effective date.

## Contact

Questions or deletion requests: **gurkansphone@gmail.com**

[![Sector Alarm](https://github.com/gjohansson-ST/sector/blob/master/logos/logo.png)](https://www.sectoralarm.se/)

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge&cacheSeconds=3600)](https://github.com/hacs/integration)
[![size_badge](https://img.shields.io/github/repo-size/gjohansson-ST/sector?style=for-the-badge&cacheSeconds=3600)](https://github.com/gjohansson-ST/sector)
[![version_badge](https://img.shields.io/github/v/release/gjohansson-ST/sector?label=Latest%20release&style=for-the-badge&cacheSeconds=3600)](https://github.com/gjohansson-ST/sector/releases/latest)
[![download_badge](https://img.shields.io/github/downloads/gjohansson-ST/sector/total?style=for-the-badge&cacheSeconds=3600)](https://github.com/gjohansson-ST/sector/releases/latest)


# Integratation to Sector Alarm
---
**Title:** "Sector Alarm"

**Description:** "Support for Sector Alarm integration with Homeassistant."

**Date created:** 2020-04-29

**Last update:** 2022-06-05

**Join the Discussion on Development:** [https://discord.gg/uvdxXChg](https://discord.gg/uvdxXChg)

---

Integrates with Swedish Sector Alarm home alarm system (most likely works in all countries serviced by Sector Alarm).
Currently supporting Alarm, Locks, Temperature and Smartplugs

## Configuration Options

Set once:

- Username: Your e-mail address linked to Sector Alarm account
- Password: Password used for app or Sector website
- Enable Temp sensors (Not recommended and turned off by default)

Options that you can change at any time:

- Update frequency: Set at minimum 60 seconds. Don't set lower as it will probably block your account
- Code: Code used to alarm and open/close door locks
- Code Format: Number of digits in code
- Log Name: Set to user which HA operates via and it will populate changed_by on state changes to the correct user name

## Installation

### Option 1 (preferred)

Use [HACS](https://hacs.xyz/) to install

### Option 2

Below config-folder create a new folder called`custom_components` if not already exist.

Below new `custom_components` folder create a new folder called `sector`

Upload the files/folders in `custom_components/sector` directory to the newly created folder.

Restart before proceeding

## Activate integration in HA

After installation go to "Integrations" page in HA, press + and search for Sector Alarm
Follow onscreen information to type username, password, code etc.
No restart needed

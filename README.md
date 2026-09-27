# Unraid Community Apps -- Jos Nienhuis

This repository contains the Unraid Community Apps templates for apps maintained by Jos Nienhuis.

## Apps

### GarageStack

An open-source vehicle monitoring dashboard for MG / SAIC electric, plug-in hybrid, and hybrid vehicles.

- **Source:** [github.com/joszz/garagestack](https://github.com/joszz/garagestack)
- **Issues / support:** [github.com/joszz/garagestack/issues](https://github.com/joszz/garagestack/issues)
- **Image:** `ghcr.io/joszz/garagestack:latest`

#### Manual install

If GarageStack is not yet visible in the Community Apps search, install it directly:

> Unraid UI -> Apps -> Install from URL -> paste the URL below

```
https://raw.githubusercontent.com/joszz/unraid-community-apps/main/templates/garagestack.xml
```

## Structure

```
templates/
  garagestack.xml   Docker container template
ca_profile.xml      Repository profile shown in Community Apps
```

## Keeping the templates in sync

`templates/garagestack.xml` is a copy. The template is maintained as
[`unraid/garagestack.xml`](https://github.com/joszz/garagestack/blob/main/unraid/garagestack.xml)
in the GarageStack repository, and the two differ only in `<TemplateURL>`, which points at each
copy itself. Never edit the copy here on its own: change the GarageStack template, then copy it
over this one and restore the `TemplateURL`, as described under "Keeping the Community Apps copy
in sync" in GarageStack's
[`documentation/RELEASING.md`](https://github.com/joszz/garagestack/blob/main/documentation/RELEASING.md).

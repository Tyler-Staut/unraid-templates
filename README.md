# Unraid Community Applications Templates

This repository contains XML templates for [Unraid Community Applications](https://forums.unraid.net/topic/38582-plug-in-community-applications/).

Each template in this repository is intended to be imported and maintained as part of a multi-template feed for Unraid users.

## Included templates

- **Astronomer** (`templates/apache_airflow_astronomer.xml`)  
  Apache Airflow (Astronomer Runtime) in standalone mode for home-lab and development use.
- **Alloy** (`templates/grafana_alloy.xml`)  
  Grafana Alloy OpenTelemetry pipeline collector.

## Repository layout

- `templates/` → Unraid CA XML templates
- `configs/` → Example/default config files referenced by templates

## Notes for Unraid CA usage

- Template XML files follow the Unraid `Container version="2"` format.
- Keep template names, icons, support links, and default paths user-friendly for CA listing.
- Use stable image tags when possible and document intended use in `Overview`.

## Adding new templates

1. Add a new XML file to `templates/`.
2. Validate XML formatting locally (for example with `xmllint --noout`).
3. Commit with a clear message describing the app/runtime being added.
4. Open a PR summarizing:
   - app purpose,
   - image/repository used,
   - ports/paths/env defaults,
   - intended deployment scope (production vs. home-lab).

## License

No license has been declared yet. If this repository is intended for broader reuse, add a license file.

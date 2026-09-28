# InfoScreen App Repository

This repository is the catalog used by InfoScreen's integrated **InfoStore**.

## Layout

- `repository.json` - catalog index read by InfoScreen.
- `applets/` - one JSON definition per applet.
- `AppIcons/` - icon assets referenced by applet definitions.

## Applet format

```json
{
  "id": "example",
  "name": "Example",
  "version": "1.0.0",
  "description": "Example InfoScreen applet.",
  "url": "https://example.com/",
  "iconUrl": "https://raw.githubusercontent.com/RavenholmZombie/InfoScreenAppRepository/main/AppIcons/example.png",
  "author": "RavenholmZombie"
}
```

The `id` must be unique and filesystem-safe. InfoScreen accepts HTTP/HTTPS applet URLs, stores installed definitions in its local `applets` directory, and caches icon assets there as well.

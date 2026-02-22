# Smart Home Floorplan Add-on for Home Assistant

**Transform your Home Assistant into a visual command center.**

Smart Home Floorplan is a 2D floorplan tool built for Home Assistant. Draw your home, place your devices, and see everything at a glance — lights, temperatures, door states, battery levels, and more — all on an interactive floorplan.

### Why?

I always wanted a nice floorplan view in Home Assistant, but drawing is not my thing — having to build it in Photoshop, SVG editors, or 3D modeling tools made it next to impossible. After many weekends trying to make my dashboard feel more like my house, I ended up building my own tool.

I wanted something that prioritized function and let me read the state of the house at a glance:

- Lights show brightness directly in the room
- Temperature shows as a subtle gradient
- Sensors show their state (e.g. "battery low")
- You can quickly see what's on, off, warm, open, etc.

It's still early, but it works as both a HA panel and a Lovelace card via this add-on.

[Website](https://getsmarthomefloorplan.com) · [Documentation](https://getsmarthomefloorplan.com/docs) · [Demo](https://getsmarthomefloorplan.com/demos) · [Discord](https://discord.gg/ScKGVyaCb7)

---

## What's in This Repo

This repository contains the **Home Assistant Supervisor add-on** for Smart Home Floorplan. The add-on runs a local service that serves the floorplan editor and viewer as an ingress panel inside Home Assistant.

### Branches

- **main**: Stable — recommended for daily use
- **edge**: Unstable — latest features, may have bugs
- **dev**: Development — experimental, likely broken

---

## Installation

> For the full step-by-step guide with screenshots, see the [Add-on Installation Docs](https://getsmarthomefloorplan.com/docs/home-assistant/add-on).

1. In Home Assistant, go to **Settings** → **Add-ons**
2. Click **Add-on Store** in the bottom right
3. Click the **⋮** menu in the top right → **Repositories**
4. Add this repository URL:
   ```
   https://github.com/loelabs-net/shf-ha-addons
   ```
5. Close the dialog. The **Smart Home Floorplan** add-on will appear in the store. Install it.

## Configuration

1. Go to [your account](https://getsmarthomefloorplan.com/account) and click **Connect to Home Assistant** to get your `propertyId` and `accessToken`.
2. In the add-on's **Configuration** tab, enter the `propertyId` and `accessToken`.
3. In the **Info** tab, enable **Start on boot** and **Auto update**, then click **Start**.
4. Click **Smart Home Floorplan** in the sidebar to open the editor.

---

## Related Repositories

Smart Home Floorplan uses three repos for Home Assistant integration:

| Repository | Description |
|---|---|
| **[shf-ha-addons](https://github.com/loelabs-net/shf-ha-addons)** | This repo — the Supervisor add-on |
| **[shf-ha-frontend](https://github.com/loelabs-net/shf-ha-frontend)** | Lovelace dashboard card for embedding floorplans |
| **[shf-ha-integrations](https://github.com/loelabs-net/shf-ha-integrations)** | Bridge integration enabling non-admin users to use floorplan cards |

If you want to add floorplan cards to your dashboards (in addition to the sidebar panel), install the frontend and integrations repos as well. See the [Card Installation Docs](https://getsmarthomefloorplan.com/docs/home-assistant/cards).

---

## Support

- Join us on [Discord](https://discord.gg/ScKGVyaCb7) for help, feedback, and discussion
- Email: support@loelabs.net
- [Full Documentation](https://getsmarthomefloorplan.com/docs)

## License

Copyright © 2025 LoeLabs LLC. All rights reserved.

See [Terms of Use](https://getsmarthomefloorplan.com/terms) for details.

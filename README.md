# HWP-workflows

A personal collection of ComfyUI workflows by [@hwprinz](https://github.com/hwprinz).  
Workflows are organised by purpose. Each entry below lists what it does, required custom nodes, and any usage notes.

---

## Workflows

### Icon-Builder — ZiT Iconbuilder RemBG ICO

**File:** `Icon-Builder/HWP-ZiT-Iconbuilder-RemBG-ICO.json`

Generates icon-ready images using the Z-Image Turbo model. The workflow includes background removal via RemBG and offers flexible output options:

- A save node outputs the generated image as **PNG or JPG**
- A second save node outputs directly as **.ICO**
- A third save node sits **before the RemBG step** — use this if RemBG removes too much detail, letting you save the raw generated image and process the background removal elsewhere (e.g. GIMP)

You can bypass any save nodes you don't need.

> **Note for Icon-Builder tool users:** The tool accepts PNG, JPG, or ICO — you only need one output format, not all three.

#### Required Custom Nodes

This workflow requires a custom node not available through the standard ComfyUI node registry:

- **apoloniartiffico-node.py** — available from [ApoloniArt/Apolonia-Nodes](https://github.com/ApoloniArt/Apolonia-Nodes)

Download the file and place it in your `ComfyUI/custom_nodes/` folder, then restart ComfyUI.

---

*More workflows will be added over time.*

### Built with 🤘 by [Hans](https://github.com/hwprinz) & with 💜 by [Apolonia](https://github.com/ApoloniArt) to reclaim your time from the mundane.

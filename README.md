# Helix Nebula — an interactive 3D interpretation

An exploration of Leo Shatz's Helix Nebula photograph, combining astronomical
imagery, catalog-derived stars, and illustrative three-dimensional geometry.

**[Open the viewer](https://eyeke2.github.io/helix3d/)** on the published GitHub Pages site.
On GitHub's repository page, use the website link in the repository's About
section after Pages is enabled; GitHub's file view does not run the player.

## Explore

- Drag horizontally or scroll over the image to change the viewing angle.
- Use the angle slider or arrow keys for precise control.
- Select **Earth view** to return to the original viewing direction.
- Select **Play sweep** for an automatic back-and-forth orbit; select **Pause**
  to stop it. Manual input also stops the sweep.
- On a touchscreen, drag horizontally over the image.

The viewing range is **−40° to +40°**. This page selects frames from a
pre-rendered video; it follows a fixed horizontal orbit rather than rendering
a freely navigable 3D scene in your browser. It includes no audio.

## What the visualization represents

The nebula's visible texture comes from Leo's color photograph, with aligned
H-alpha imagery helping identify faint outer emission. Its broad geometry is
adapted from the Chandra team's printable version of the INAF / Sal Orlando
Helix model. The extended outer envelope and 51 internal radial features use
illustrative depths and thicknesses chosen for this visualization.

The star field contains 1,341 mapped Gaia DR3 sources. Approximate stellar
distances were estimated from catalog parallaxes and strongly compressed for
display. Star colors follow Gaia BP−RP photometry, with enhanced saturation;
they are not derived from measured spectra. Apparent star sizes are adjusted
for visibility, not shown to physical scale.

**This is a blend of astronomical data and artistic interpretation, not a
measured three-dimensional reconstruction.** The changing view represents
camera motion around a fixed model, not nebular expansion or stellar motion.

## Files and hosting

| File | Purpose |
| --- | --- |
| `index.html` | Player, controls and embedded Earth-view poster |
| `helix-orbit.mp4` | 401 rendered views, 1920 × 1388, H.264, about 15.7 MB |
| `README.md` | Description, instructions, credits and licensing scope |
| `LICENSE` | CC BY-NC-SA 4.0 notice and complete legal text for creative content |
| `LICENSE-CODE` | MIT license for the player code |

Keep these files together at the repository root. For GitHub Pages, select
**Settings → Pages → Deploy from a branch**, choose the branch containing
these files and **/(root)**, then save. Add the published site address to the
repository's About section. No build step or third-party JavaScript libraries
are required. For local use, open `index.html` with the MP4 beside it.

Only finished imagery and the lightweight player are distributed here. The
underlying meshes, original astronomy files, star catalog and rendering tools
are not included. The video contains 0.2° angular steps; its 13.367-second
duration is an angle lookup sequence. The player's automatic sweep uses its
own slower timing. Seeking responsiveness depends on the device and connection.

## Credits

- **Imaging, creative direction and visualization:** Leo Shatz
  ([spinlock on AstroBin](https://app.astrobin.com/u/spinlock?i=l7pmzx)).
- **Reference geometry:** INAF / Sal Orlando; printable adaptation by the
  Chandra team. [The Helix Nebula in 3D](https://chandra.harvard.edu/deadstar/helix.html).
  The reference geometry was adapted to Leo's image and supplemented with
  illustrative internal globules and an extended outer envelope.
- **Stellar catalog:** ESA / Gaia, Gaia Data Processing and Analysis Consortium
  (DPAC), Data Release 3.
- **AI-assisted modeling, visualization and software development:** OpenAI
  Codex (GPT-6 Astra), directed and reviewed by Leo Shatz.

These credits acknowledge contributions and sources; they do not imply
endorsement by the named institutions or services.

## Licensing

Copyright © 2026 Leo Shatz, for his copyrightable contributions.

**Imagery and explanatory text:** Leo's contributions to the rendered video,
embedded poster, and explanatory text are licensed under
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)
(**CC BY-NC-SA 4.0**). See [LICENSE](LICENSE) for the scope and full terms.
In summary, noncommercial sharing and adaptation are permitted with appropriate
credit, a license link, and identification of changes; shared adaptations must
use the same license or an allowed compatible license. The legal text governs.
CC BY-NC-SA does not require supplying the unpublished meshes, source images
or rendering tools. The license cannot be revoked for compliant recipients.

**Player code:** The HTML markup, CSS and JavaScript implementing the player
are licensed under [MIT](LICENSE-CODE). This permits commercial reuse of the
player code, but does **not** grant commercial-use permission for the video,
embedded poster or explanatory text. Remove or replace those assets if reusing
the player outside their license terms.

**Third-party material:** These licenses grant only rights Leo is entitled to
grant. They do not relicense the INAF / Sal Orlando reference model, the
Chandra adaptation, Gaia data, logos, trademarks, or other third-party material;
any applicable upstream rights and terms remain separate. No restrictions are
added to public-domain elements or uses allowed by law.

Chandra's source page identifies the model's creators, but an explicit
STL-specific reuse license was not identified on the linked pages. Its
[usage policy](https://chandra.harvard.edu/photo/image_use.html) distinguishes
Chandra-produced content from externally supplied material. Attribution is not
a substitute for any permission required from upstream rights holders; the
licenses in this repository do not certify clearance of those rights.

### Suggested attribution

> Helix Nebula — an interactive 3D interpretation, © Leo Shatz, CC BY-NC-SA 4.0
> (Leo Shatz's imagery and creative contributions). Reference geometry:
> INAF / Sal Orlando, printable adaptation by the Chandra team. Stellar data:
> ESA / Gaia / DPAC. Player code: MIT.

When sharing, include a link to the source repository or published viewer and
the CC license, retain relevant notices, and describe any changes you made.
The supplied media carries a © Leo Shatz watermark at 25% opacity.

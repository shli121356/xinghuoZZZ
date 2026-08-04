# Logo Replacement Design

## Goal

Replace the homepage's current top-left icon and adjacent brand text with the supplied Xinghuo logo while preserving the existing dark warm-ember visual treatment.

## Design

- Use the supplied transparent PNG as the source asset.
- Crop transparent outer padding so the asset can be sized predictably.
- Recolor the white mark into the site's existing warm gold/orange range instead of displaying it as plain white.
- Apply the existing orange drop shadow and a restrained warm container glow.
- Replace the current `.mark` image and the separate `brand-title`/`brand-sub` text with one complete logo lockup.
- Use the same processed asset for the page favicon so the browser tab stays consistent.

## Responsive Behavior

- Desktop header logo height: approximately 78px.
- Mobile header logo height: approximately 64px.
- The logo must remain contained within the header and must not overlap the status pill or hero content.

## Scope

Only the homepage branding asset, its immediate header markup/styles, and the favicon are in scope. No navigation destinations, copy, API behavior, or other visual sections change.

## Verification

- Load the homepage through the existing local static server and confirm the logo asset is served.
- Capture desktop and mobile screenshots to verify the logo is visible, warm-colored, and contained.
- Confirm the homepage and favicon requests return HTTP 200.

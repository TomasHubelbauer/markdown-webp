# MarkDown Animated WebP

This repository serves as a test of animated WebP support in GitHub and VS Code
MarkDown previews when a WebP image is embedded in the MarkDown document as an
image.

![](test.webp)

## Support

WebP has good, but not amazing browser support:

https://caniuse.com/#feat=webp

The lack of support in Safari is a bummer.

- Supported in VS Code MarkDown preview
- Supported in GitHub MarkDown preview

## Alternatives

For animation in MarkDown, the current options include:

- SVG with CSS animation: vector, performant, well compressible in transit
- GIF: raster, old, big, slow and ugly, should not be used for anything ever

The following are unfortunately not well supported:

- MP4: `video` is not supported in MarkDown and embedding as an image won't work
- APNG: might be an option actually: https://caniuse.com/#feat=apng
- MNG: ?

## Takeaway

Use SVG whenever possible, add animation using CSS animations where beneficial.

## To-Do

### Ensure the MP4 claim is correct

### Test out APNG and MNG in GitHub and VS Code MarkDown previews

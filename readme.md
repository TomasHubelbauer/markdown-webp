# MarkDown Animated WebP

This repository serves as a test of animated WebP support in GitHub and VS Code
MarkDown previews when a WebP image is embedded in the MarkDown document as an
image.

![](test.webp)

Test image courtesy of [Mathias Bynens](https://mathiasbynens.be/demo/animated-webp).

## Support

https://caniuse.com/#feat=webp

- [x] Supported in web browsers
- [x] Supported in VS Code MarkDown preview
- [x] Supported in GitHub MarkDown preview

## Alternatives

For animation in MarkDown, the current options include:

- SVG with CSS animation: vector, performant, well compressible in transit
- GIF: raster, old, big, slow and ugly, should not be used for anything ever

The following are unfortunately not well supported:

- MP4: GitHub supports video, VS Code preview I don't know
  https://github.blog/2021-05-13-video-uploads-available-github
- APNG: might be an option actually: https://caniuse.com/#feat=apng
- MNG: no support information on CanIUse, likely not well supported

## Takeaway

- Use SVG when the animation benefits from vector rendering
- Use WebP for static images or raster animations
- Use videos when targetting GitHub preview, will show up as path text elsewhere

## To-Do

### Compare APNG and WebP size and ease of generation to focus recommendation

I am leaning towards WebP as it is newer and is well supported now, but it would
be good to put some numbers behind this.

### Test out whether VS Code preview can handle video too now

GitHub rolled this out recently, maybe VS Code has as well or there is an
extension to recommend?

### Test out APNG and MNG in GitHub and VS Code MarkDown previews

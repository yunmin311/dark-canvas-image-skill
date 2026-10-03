# 生成示意素材的实际请求

三次内建 image_gen 调用，transparent_background=false，未作后期处理。初稿两张输入为 CC0 亚麻 AO；修正输入为初稿磨损片与用户黑白枯枝月作品（仅观察表面旧痕，作品未纳入包）。以下为完整 prompt；图片角色通过真实 referenced_image_paths 传入。选择结果见 [generated-guides.json](generated-guides.json)。

## worn

```text
Edit the supplied real linen texture into a neutral grayscale material reference only, a front-facing closeup of aged primed painting canvas. Preserve its fine straight warp/weft fabric structure. Add restrained irregular old discoloration and a sparse scatter of tiny pale pigment losses and rubbed bare spots. Quiet large intact areas, low contrast, asymmetrical natural wear distributed unevenly, very few fine linear scuffs. Flat thin primer/pigment integrated with the cloth; not bare coarse burlap. This is a texture reference, not an artwork: no scene, figures, landscape, lettering, object, picture frame or border. No curled ornamental etching, thick paint, crackle mosaic, stone or paper. Mid-gray monochrome without colored tint. The entire image is the canvas material, not a photograph of a stretched canvas in a room.
```

## distressed

```text
Edit the supplied real linen texture into a neutral grayscale closeup material reference of worn old primed painting canvas. Preserve fine straight horizontal/vertical weave, softened by thin old pigment and primer. Compared with clean canvas include clearly visible but quiet irregular rubbed pale losses, localized thin worn patches, a few small darker age marks and isolated fine scratches. Retain plenty of continuous intact fabric between marks; the damage does not form evenly repeated dots or decorative curls. Losses reveal underlying cloth, not a wall or paper. No tears or holes through the whole image, no burnt edge or antique picture-frame border. Flat diffuse lighting and low relief; mid-gray monochrome, no color cast. Material fills the frame, no subjects, text, artworks, paint blobs, thick impasto, coarse burlap, embossed swirls, stone cracks or paper fibers.
```

## distressed correction

```text
Edit image1 into a blank material-reference image of worn primed painting canvas. Image1 supplies fine straight linen fibers; image2 supplies ONLY the scale and quiet irregularity of old discoloration, rubbed pigment loss and scratches visible in its canvas surface, NOT its tree, moon, black/white scene, composition or exact blemish locations. The material fills the entire frame. IMPORTANT: show a thin continuous MATTE MID-GRAY PRIMER/PIGMENT layer over the weave, hiding most stark exposed threads. Broad very low-contrast patches of uneven aging, a few small rubbed pale pigment losses, some isolated tiny flecks and thin scratches, with large quiet intact areas. More visible and varied wear than image1, but no dramatic damage. Fine subdued straight cross-weave remains below the thin pigment in all intact areas. No scene, tree, branch, moon, object, text, frame, vignette or border. No bare raw burlap, high-contrast coarse loose threads, stone, plaster, paper grain, curled decorative marks, crackle web, thick impasto, burnt edges or holes. Neutral grayscale material only; random natural locations, not a copy of image2's wear pattern.
```

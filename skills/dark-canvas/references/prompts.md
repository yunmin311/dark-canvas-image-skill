# 图生图请求模板

下面是请求内容，不是图像工具的新参数。按本次选择替换括号，只保留需要的表达；不要把选项全部写进同一张图。源图已给定时不用新建合成场景。

## 基本编辑

先用简短请求，实际附入原照片和选定作品，不用作者名代替作品：

```text
Apply the visual finish of image 2 to the photograph in image 1. Keep image 1's [source colors/exposure/content/crop]. Borrow image 2's [selected form, background and surface qualities], not its palette or subjects. The result remains this photograph with the reference's understated poetic finish. [Only the most relevant avoid condition.]
```

需要进一步区分角色/区域时再使用以下展开版本；不能把所有可选短句堆进去。

```text
Edit image 1. Keep its subject, main arrangement, specified object counts, original crop and source palette: [main colors and their relative areas]. Only unify small tonal variations within those original color families.
Image 2 is the artwork reference for [chosen form/edge treatment], [surface/wear] and [vignette level], not for its subject, composition or palette.
[If needed: Image 3 is the selected material reference for weave/wear morphology only, not its gray color or contrast.]
Apply [retained photographic shapes / economical Chinese-brush-like handling / clean flat cut-paper-like silhouettes / selective directional softening] to [regions]. Match the reference's quiet background and unified tonal fields. [Chosen canvas/wear treatment.] [Chosen vignette treatment, or none.]
Preserve natural irregularity and useful source details. Do not invent props, change the crop, globally recolor, add glossy 3D modeling, ornate texture or a theatrical antique frame. Do not introduce paper layers or paper grain merely because silhouettes are cut-paper-like. Deliver one finished poetic image.
```

## 可选表达短句

- 毛笔：`Economical directional forms with tapered endings, a few restrained dry-brush edges; no scattered oil-paint dabs or modeled shiny highlights.`
- 剪影：`Keep recognizable crisp silhouettes and meaningful small branches; simplify internal shading into calm flat dark forms. No layered paper sculpture or added paper material.`
- 保留摄影：`Retain the source's natural shapes and important detail; reduce harsh local contrast, integrate image and subtle surface. Do not redraw as a synthetic studio illustration.`
- 雾化/拖影：`Keep selective softening in [region/direction], while [recognition-critical shape] stays readable. Not uniform blur.`
- 细布：`Fine straight woven structure quietly under the image, thin matte surface, no curly engraving or coarse burlap; scale from the artwork reference.`
- 局部旧痕：`Sparse uneven old staining, a few rubbed thin spots and isolated small scuffs, with large continuous quiet areas. No uniform dirt overlay.`
- 磨损残破：`Localized pigment losses, tiny exposed-ground flecks and a few irregular scratches, matched to the artwork's scale; intact continuous cloth remains. No large holes, burn edges, decorative crackle or plaster chips.`
- 晕影：`[Subtle/visible] broad soft edge falloff matching the artwork, within source colors, no hard black corners or border; preserve the original crop.`
- 无晕影/无做旧：必要时写明 `Keep edges open; no added vignette.` / `Clean cloth surface; no added age marks.`，不默认给每张加入这些限制。

## 定向修正

```text
Correct only [observed problem] in this candidate, using the original source again where content or colors drifted. Preserve [already correct content/color/form/material]. Match [chosen reference property] in [region]. Keep [wear/vignette] only at its selected level; do not change other style choices. No new props or crop changes.
```

修正必须来自实际看图，不能因换了模板就记为通过。完整实际请求、输入顺序、输出路径与每轮观察保存到任务记录；未出图不写成“已验证”。

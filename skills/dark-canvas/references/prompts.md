# 简短提示词与输入分工

看过实际图片后填写；新图与编辑分开，不拼入互相冲突的风格名。素材与输入路径使用真实接口，不虚构强度或配色参数。

## 编辑

```text
Edit image 1. Keep its [main colors, warm/cool relationships, color proportions], [subject/counts], [crop and main arrangement]. Only modest tonal unification within the existing palette is allowed.
Image 2 supplies Chinese brush-painting-like economy and unified background fields, not its colors or subjects. Image 3 supplies real linen warp/weft structure, not its grayscale color or contrast.
Render the existing subject as economical ink-brush-like pigment shapes with restrained tapered/dry-brush handling on primed oil canvas. Unify quiet background color fields within their original color families. Suppress camera sharpness, glossy modeling and fussy microdetail. Fine low-contrast weave integrated with pigment.
No watercolor blooms/paper staining, ornamental curls, coarse cloth, added motifs or text. Keep [explicit exact-content requirements, if any]. Deliver one finished image.
```

## 新图

```text
Create one [format] image of [requested subject/counts and arrangement]. Palette: [user-selected or explicitly chosen reference colors].
Quiet unified background fields, economical Chinese brush-painting-like pigment shapes and restrained brush ends on primed oil canvas. Fine actual linen structure is a material reference only; no borrowing its gray/white color.
Avoid photographic microdetail, watercolor/paper effects, ornamental etched texture and added motifs. Deliver the completed image.
```

## 定向修正

```text
Observed mismatch: [what is actually wrong]. Restore/correct [one property] using [source/reference role]. Keep [already correct colors, content and format]. Do not carry forward [the failed version's specific distortion].
```

记录完整实际提示词、每张输入的角色、各版路径及逐项观察。水印、身份、色彩与材质是否成功，只能依据实际文件检查，不能由提示词保证。

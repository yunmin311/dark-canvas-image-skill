> 历史 v0.6.0 记录，保留供追溯；当前逐图状态见 [验收记录](../skills/dark-canvas/references/validation-status.md)。

# v0.6.0 真实照片的实际图生图请求

一张用户真实柳岸照片，共三次实际编辑；没有合成跨主题场景。内建 image_gen，transparent_background=false，照片及结果仅本地保存。下面是完整实际 prompt；输入用真实 referenced_image_paths 传入，公开记录仅描述角色，不公开照片或个人绝对路径。

## 第 1 版

输入顺序：原照片 / 用户竹叶鸟作品 / 真实亚麻 AO。

```text
Style-transfer image1 using image2's photographic-art treatment. Keep image1's original 4:3 crop, willow branches, treeline, reflections, small lights and dark warm-neutral gray / near-black green colors. Image2 is ONLY the reference for its calm continuous background, elegant dark leaf/branch silhouettes and fine canvas surface, not its bird, composition or beige hue. Image3 is ONLY real fine linen weave morphology. Keep the natural shapes of the original photograph. Give it the quiet image-on-canvas quality of image2, integrating subtle fine straight weave through sky, water and branches, unifying small background tonal variations without changing the overall palette or lifting exposure substantially. Branch and leaf contours may remain clean like the reference; simplify harsh microcontrast, not the scene. Do not repaint as a flat synthetic illustration, add oil-paint dabs, paper sculpture, watercolor blooms, new objects, ornate curls, vignette or aged damage. One finished poetic photographic canvas image.
```

## 第 2 版

输入顺序：重新附原照片 / 用户已认可 Creative OS 植物原成图。

```text
Edit image1 with the visual finish of image2, the user's previously successful Creative OS image. Image1 is the real photograph to keep: original willow canopy, shoreline, reflection, lights, crop and dark warm-gray / near-black green palette. Image2 supplies only its quiet photographic silhouettes, continuous matte tone, finely integrated cloth surface and subtle uneven old patina, not its reeds, kite, layout or warm gold palette. Keep the photograph's natural shapes and irregularity. Borrow the reference's restrained image-on-canvas finish, with its small-scale fine weave rather than a large raw-fabric mesh. Keep the main source colors and relative brightness; no global brightening or recoloring. A very light broad edge falloff is acceptable, without dark hard corners. No invented subjects, oil-paint dabs, shiny 3D modeling, paper layers, watercolor staining, ornate curled texture or drastic simplification. A poetic photographic image with the same understated finish as image2.
```

## 第 3 版

输入顺序：重新附原照片 / 用户竹叶鸟作品（不另附材质）。

```text
Apply the visual finish of image2 to the photograph in image1. Preserve image1's original dark neutral-gray/black-green colors, exposure, willow canopy, shoreline, reflection, lights and 4:3 crop. Use image2 for its calm even background, clean natural silhouettes and subtle fine canvas grain. The result remains the same photograph with this understated finish. Do not borrow image2's beige color or bird, brighten into sepia, redraw as an illustration, add curled paint marks or show coarse raw cloth.
```

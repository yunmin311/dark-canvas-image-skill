# 可执行提示词

将方括号替换为本次要求，删除不适用语句。**一次只用一个变体。** 固定提示词不保证固定结果。

下面三段模板均于 2026-10-02 用内建 `image_gen` 实测通过，对应 `examples/validation.md` 的记录。

## 从零生成（默认暖金亚麻，实测通过）

```text
Create one original landscape-format image, 3:2, in the visual family of the two reference images: an oil-painting-like, quiet poetic nature scene.

Do not copy either reference scene. Build a new one.

Mood: hushed, still, solitary, meditative. Nothing dramatic, nothing heroic.

Medium and surface: an oil painting on woven linen canvas. Clearly visible fine linen canvas weave and fabric grain, continuous across the entire image including sky, water and silhouettes. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than by line. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette: warm golden ochre and amber light in the sky, smoky neutral gray clouds, muted olive and sepia in the middle distance, deep near-black charcoal silhouettes. Very low saturation, except one small restrained warm accent. No vivid blue, no cyan, no orange-teal grading, no HDR punch.

Composition: 3:2 landscape, horizon low. Sky and luminous mist fill roughly two thirds of the frame. A low band of soft hazy hills recedes in layers, each paler than the one in front. Dark near-black foliage masses enter from the bottom and lower corners as natural framing. One small loose flock of five or six tiny distant birds crosses the open upper sky as the only sharp accent. Everything else stays soft and atmospheric. Asymmetric, unhurried framing with generous empty space.

Avoid: golden sunburst, central spotlight, epic cinematic landscape, HDR crispness, heavy saturation, uniform global blur, thick painterly impasto, text, signature, border, collage.
```

## 烟灰单色变体（实测通过）

```text
Create one original 3:2 fine-art image: a monochrome black and white oil painting on woven linen canvas, quiet and meditative.

Do not copy the reference scene. Build a new one.

Mood: hushed, still, solitary, a long silent evening. Nothing dramatic.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value instead of outline. Matte, no gloss. Not a glossy digital photograph, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette: near-monochrome. Deep charcoal blacks, layered smoke-gray midtones, soft luminous pale gray in the sky. No color cast at all, no sepia, no warm tone. One small bright white disc high in the sky as the single point of light. The lightest area is a soft halo around it, fading outward into gray.

Composition: 3:2 landscape, low horizon. Sky fills roughly two thirds. A cluster of thin bare branches rises from the bottom edge, slightly left of center, with a second smaller cluster at the right. One small bright disc sits in the upper middle, clear of the branches. Generous empty space, asymmetric, unhurried.

Avoid: color, sepia, golden sunburst, central spotlight, epic cinematic landscape, HDR contrast, uniform global blur, thick impasto, text, signature, border, collage.
```

## 将照片转换为亚麻油画（实测通过）

```text
Edit image 1, the source photograph. Image 2 is a style reference only for palette, mood and surface — never for scene content.

Keep the source's exact 3:2 crop, camera position, perspective and horizon. Preserve every object and its position: [列出查看原图后确认的地标／人物／物件]. Do not add birds, boats, buildings or any object that is not in the source.

Repaint the scene as an oil painting on woven linen canvas. Apply a clearly visible fine linen canvas weave and fabric grain, continuous across sky, water and silhouettes. Use soft blended painterly tonal masses and gentle feathered edges, forms modelled by value rather than outline. Matte surface, no gloss, no varnish.

Palette: warm golden ochre and amber light in the sky, smoky neutral gray clouds, muted olive and sepia in the middle distance, deep near-black charcoal shadows. Very low saturation. [若有彩色物件] 其颜色转为低饱和氧化土色，不是鲜艳点缀。

Keep [关键结构：屋脊、门窗、轮廓] readable. Soften only the distant background. No golden sunburst, no central spotlight, no dramatic new cloud structures, no uniform blur.

Avoid: added objects, thick raised impasto, glossy digital photo look, vivid blue, orange-teal grading, HDR contrast, text, signature, border, collage.
```

**这是重绘，不是滤镜。** 已知风险：模型会重绘天空云形并轻微改动细节，因此不要宣传为无损／逐像素保真。

## 交付记录

写出：最终提示词、每张输入的角色、生成／编辑工具、输出路径、对照参考的逐项偏差、以及**右下角是否出现工具水印**。

隐私路径可留在本地记录；公开记录使用仓库相对路径，不放分享令牌或个人文件夹地址。

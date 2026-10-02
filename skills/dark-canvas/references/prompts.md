# 可执行提示词

将方括号替换为本次要求，删除不适用语句。**一次只用一个色域。** 固定提示词不保证固定结果。

下面五段模板均于 2026-10-02 用内建 `image_gen` 实测通过，对应 `examples/validation.md`。

**用法**：先确定场景与光线 → 选对应的色域模板 → 在`Palette` 段按该色域填色。**不要跨色域混填**，也不要把暖金当成万能默认。

---

## 模板 A · 暖金夕照（实测通过）

对应 `skills/dark-canvas/assets/calibrated-ochre-canvas.jpg`。

```text
Create one original landscape-format image, 3:2, in the visual family of the reference images: an oil-painting-like, quiet poetic nature scene.

Do not copy the reference scene. Build a new one.

Mood: hushed, still, solitary, meditative. Nothing dramatic, nothing heroic.

Medium and surface: an oil painting on woven linen canvas. Clearly visible fine linen canvas weave and fabric grain, continuous across the entire image including sky, water and silhouettes. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than by line. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette driven by the scene [late golden light]: warm golden ochre and amber light in the sky, smoky neutral gray clouds, muted olive and sepia in the middle distance, deep near-black charcoal silhouettes. Very low saturation, except one small restrained warm accent. No vivid blue, no cyan, no orange-teal grading, no HDR punch.

Composition: 3:2 landscape, horizon low. Sky and luminous mist fill roughly two thirds of the frame. A low band of soft hazy hills recedes in layers, each paler than the one in front. Dark near-black foliage masses enter from the bottom and lower corners as natural framing. One small loose flock of five or six tiny distant birds crosses the open upper sky as the only sharp accent. Everything else stays soft and atmospheric. Asymmetric, unhurried framing with generous empty space.

Avoid: golden sunburst, central spotlight, epic cinematic landscape, HDR crispness, heavy saturation, uniform global blur, thick painterly impasto, text, signature, border, collage.
```

## 模板 B · 冷蓝夜渡（实测通过）

对应 `calibrated-dusk-blue.jpg`。**示范冷色场景如何只留一处暖色。**

```text
Create one original 3:2 fine-art image: a quiet oil painting on woven linen canvas, a dusk fishing scene.

Do not copy the reference scene. Build a new one.

Palette driven by the scene [twilight]: deep cool blue-teal twilight, slate blue water, muted blue-gray sky. Low saturation throughout. One small restrained warm accent only: an orange-red life ring on the boat and a faint warm lamp glow, small and localized, nothing else warm. Deep near-black boat hull and figures.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than outline. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a digital grid.

Content and composition: a small wooden fishing boat with a simple canopy moored near the right bank, two small figures in pale shirts seated inside, seen at a distance. Reeds and a low dark bank frame the left edge. Open water fills the middle, a low hazy far shore behind. Sky fills roughly two thirds. Everything soft and atmospheric except the boat, which carries the single point of focus. Asymmetric, unhurried, generous empty space, quiet and solitary mood.

Avoid: warm golden sky, orange sunset, teal-orange grading, vivid saturation, HDR contrast, glossy photo look, thick impasto, text, signature, border, collage.
```

## 模板 C · 清晨薄雾（实测通过）

对应 `calibrated-morning-cream.jpg`。

```text
Create one original 3:2 fine-art image: a quiet oil painting on woven linen canvas, an early morning lake scene with wooded hills.

Do not copy the reference scene. Build a new one.

Palette driven by the scene [early morning]: soft warm cream and pale gold light in the sky, hazy warm gray clouds, muted natural olive and deep green foliage on the hills, a cool gray-green water surface. Low saturation, gentle and restrained, nothing vivid. Deep near-black accents only in the closest foreground vegetation.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than outline. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a digital grid.

Content and composition: a wide calm lake, a small wooden boat with a pale canopy near the left bank, a few tiny indistinct figures aboard. Forested hills recede behind in overlapping layers, each paler and softer than the one in front, fading into morning haze. A cluster of dark reeds enters the bottom right corner as natural framing. Sky fills roughly two thirds. One small flock of distant birds crosses the open sky. Asymmetric, unhurried, generous empty space, serene and solitary mood.

Avoid: vivid blue sky, orange sunset, teal-orange grading, oversaturated green, HDR contrast, glossy photo look, thick impasto, text, signature, border, collage.
```

## 模板 D · 烟灰单色（实测通过）

对应 `calibrated-night-mono.jpg`。

```text
Create one original 3:2 fine-art image: a monochrome black and white oil painting on woven linen canvas, quiet and meditative.

Do not copy the reference scene. Build a new one.

Mood: hushed, still, solitary, a long silent evening. Nothing dramatic.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value instead of outline. Matte, no gloss. Not a glossy digital photograph, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette: near-monochrome. Deep charcoal blacks, layered smoke-gray midtones, soft luminous pale gray in the sky. No color cast at all, no sepia, no warm tone. One small bright white disc high in the sky as the single point of light. The lightest area is a soft halo around it, fading outward into gray.

Composition: 3:2 landscape, low horizon. Sky fills roughly two thirds. A cluster of thin bare branches rises from the bottom edge, slightly left of center, with a second smaller cluster at the right. One small bright disc sits in the upper middle, clear of the branches. Generous empty space, asymmetric, unhurried.

Avoid: color, sepia, golden sunburst, central spotlight, epic cinematic landscape, HDR contrast, uniform global blur, thick impasto, text, signature, border, collage.
```

---

## 模板 E · 照片转换为亚麻油画（实测通过）

**色彩跟原图光线走**，不要强加暖金。转换前先看原图，判断它属于哪个色域，再决定 `Palette` 段怎么写。

```text
Edit image 1, the source photograph. Image 2 is a style reference only for palette, mood and surface — never for scene content.

Keep the source's exact [aspect ratio] crop, camera position, perspective and horizon. Preserve every object and its position: [列出查看原图后确认的地标／人物／物件]. Do not add birds, boats, buildings or any object that is not in the source.

Repaint the scene as an oil painting on woven linen canvas. Apply a clearly visible fine linen canvas weave and fabric grain, continuous across sky, water and silhouettes. Use soft blended painterly tonal masses and gentle feathered edges, forms modelled by value rather than outline. Matte surface, no gloss, no varnish.

Palette driven by the source's own light: [按原图光线填写——晨雾奶白／夕照暖金／夜渡冷蓝／单色烟灰]。Keep the source's overall color temperature; do not shift a cool scene toward gold. Very low saturation. [若有彩色物件] 其颜色转为低饱和氧化土色，不是鲜艳点缀。To one small restrained warm accent only, no more.

Keep [关键结构：屋脊、门窗、轮廓] readable. Soften only the distant background. No golden sunburst, no central spotlight, no dramatic new cloud structures, no uniform blur.

Avoid: added objects, thick raised impasto, glossy digital photo look, vivid blue, orange-teal grading, HDR contrast, text, signature, border, collage.
```

**这是重绘，不是滤镜。** 已知风险：模型会重绘天空云形并轻微改动细节，不要宣传为无损／逐像素保真。

## 交付记录

写出：最终提示词、**选定的色域及依据（什么时间／什么光线）**、每张输入的角色、生成／编辑工具、输出路径、对照参考的逐项偏差、以及右下角是否出现工具水印（预期出现，属工具 AI 标识，不去除）。

隐私路径可留在本地记录；公开记录使用仓库相对路径，不放分享令牌或个人文件夹地址。

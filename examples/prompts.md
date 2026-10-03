> v0.2/v0.3 历史调用记录：接口参数与水印观察属于当时宿主，不是当前 Codex 内建工具接口说明。新调用见 [当前图生图模板](../skills/dark-canvas/references/prompts.md)。

# 本次实际调用的提示词

工具：内建 `image_gen`；日期：2026-10-02；size `1536x1024`，quality `high`。
以下为**实际调用时的完整文本**。第三方参考图路径改写为本地说明；公开仓库不含这些文件。

## 1. 旧中性灰配方复现（对照用）

输入角色：图 1 = 阴云飞鸟（色域、表面），图 2 = 枝叶（剪影、细纹）。输出：`legacy-neutral-recipe.jpg`。

```text
Generate a new original 3:2 photograph-style image. Use image 1 only as the reference for neutral gray tonality, cloudy light, fine flat print surface and restrained edge wear. Use image 2 only as the reference for natural dark foliage edges and the subtle fine surface texture. Do not reproduce either reference composition. New scene: looking upward across a quiet rural valley, uneven distant tree silhouettes occupy only a narrow bottom band, a close sparse leaf branch enters the top right, one very small distant bird in the left third of the open sky. Mostly sky, natural irregular overcast cloud layers, pale diffuse silver-gray top sky gradually deepening to charcoal cloud at lower right, no golden sunburst or central dramatic spotlight. Neutral monochrome with only a trace of warm gray, truly black silhouettes against lighter sky; photographic tonal gradients and restrained softness. Closely match the reference's fine flat softly visible crosshatched print surface: tiny evenly distributed fiber/dot-like marks, no raised threads, no heavy canvas or burlap, no painterly marks, texture must be quieter than the imagery and uninterrupted across the frame. Very faint irregular print wear near extreme edges, no drawn frame or heavy vignette. A candid atmospheric photographic observation, simple unresolved framing, not an epic fantasy landscape, not a painting. No warm sepia or amber grading, no orange leak, no added objects, no text, no signature, no watermark, no collage.
```

**结果**：织纹与阴云成立，但整体偏冷灰、金调缺失，且右下角出现「AI生成」水印。保留仅作对照。

## 2. 暖金亚麻默认配方（修正后，通过）

输入角色：图 1 = 暖金群鸟／云（色域、表面），图 2 = 灰绿山峦（层次、留白）。输出：`../skills/dark-canvas/assets/calibrated-ochre-canvas.jpg`。

```text
Create one original landscape-format image, 3:2, in the visual family of the two reference images: an oil-painting-like, quiet poetic nature scene.

Do not copy either reference scene. Build a new one.

Mood: hushed, still, solitary, meditative. Nothing dramatic, nothing heroic.

Medium and surface: an oil painting on woven linen canvas. Clearly visible fine linen canvas weave and fabric grain, continuous across the entire image including sky, water and silhouettes. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than by line. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette: warm golden ochre and amber light in the sky, smoky neutral gray clouds, muted olive and sepia in the middle distance, deep near-black charcoal silhouettes. Very low saturation, except one small restrained warm accent. No vivid blue, no cyan, no orange-teal grading, no HDR punch.

Composition: 3:2 landscape, horizon low. Sky and luminous mist fill roughly two thirds of the frame. A low band of soft hazy hills recedes in layers, each paler than the one in front. Dark near-black foliage masses enter from the bottom and lower corners as natural framing. One small loose flock of five or six tiny distant birds crosses the open upper sky as the only sharp accent. Everything else stays soft and atmospheric. Asymmetric, unhurried framing with generous empty space.

Avoid: golden sunburst, central spotlight, epic cinematic landscape, HDR crispness, heavy saturation, uniform global blur, thick painterly impasto, text, signature, border, collage.
```

**结果**：织纹在缩略图可见、暖金主调成立、油画感成立、群鸟母题到位。右下角仍有「AI生成」水印。

## 3. 烟灰单色变体（通过）

输入角色：图 1 = 单色月／枯枝（色域、表面）。输出：`../skills/dark-canvas/assets/calibrated-monochrome.jpg`。

```text
Create one original 3:2 fine-art image: a monochrome black and white oil painting on woven linen canvas, quiet and meditative.

Do not copy the reference scene. Build a new one.

Mood: hushed, still, solitary, a long silent evening. Nothing dramatic.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value instead of outline. Matte, no gloss. Not a glossy digital photograph, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette: near-monochrome. Deep charcoal blacks, layered smoke-gray midtones, soft luminous pale gray in the sky. No color cast at all, no sepia, no warm tone. One small bright white disc high in the sky as the single point of light. The lightest area is a soft halo around it, fading outward into gray.

Composition: 3:2 landscape, low horizon. Sky fills roughly two thirds. A cluster of thin bare branches rises from the bottom edge, slightly left of center, with a second smaller cluster at the right. One small bright disc sits in the upper middle, clear of the branches. Generous empty space, asymmetric, unhurried.

Avoid: color, sepia, golden sunburst, central spotlight, epic cinematic landscape, HDR contrast, uniform global blur, thick impasto, text, signature, border, collage.
```

**结果**：纯黑白无色偏，织纹为该变体最强线索。右下角仍有水印。

## 4. 照片转换为亚麻油画（通过，云形重绘 FAIL）

输入顺序：`transfer-source.jpg`（编辑目标，本文件同目录）；图 2 = 暖金群鸟／云（色域、表面）。输出：`transfer-canvas.jpg`。

```text
Edit image 1, the source photograph. Image 2 is a style reference only for palette, mood and surface — never for scene content.

Keep the source's exact 3:2 crop, camera position, perspective and horizon. Preserve every object and its position: the leafy tree entering from the left edge, the white wooden boathouse with its pitched roof on the right bank, its doorway and window, the diagonal wooden dock running from the lower right toward the centre, exactly ONE small rowing boat moored at the dock, the rocks along the bank, and the layered distant hills. Do not add birds, boats, buildings or any object that is not in the source.

Repaint the scene as an oil painting on woven linen canvas. Apply a clearly visible fine linen canvas weave and fabric grain, continuous across sky, water and silhouettes. Use soft blended painterly tonal masses and gentle feathered edges, forms modelled by value rather than outline. Matte surface, no gloss, no varnish.

Palette: warm golden ochre and amber light in the sky, smoky neutral gray clouds, muted olive and sepia in the middle distance, deep near-black charcoal foliage shadows and dock. Very low saturation. The boat's red becomes a small subdued oxidized-earth tone, not a vivid accent. The boathouse walls stay relatively lighter but lose all clean white.

Keep the roof, door, window, boat outline, dock posts and planks readable. Soften only the distant hills and cloud edges. No golden sunburst, no central spotlight, no dramatic new cloud structures, no uniform blur.

Avoid: added objects, thick raised impasto, glossy digital photo look, vivid blue, orange-teal grading, HDR contrast, text, signature, border, collage.
```

**结果**：船屋／栈桥／单船结构保留，亚麻油画表面与暖金色域成立。天空仍被重绘（与旧版一致），不宣传为无损。右下角仍有水印。

## 水印观察（第一轮）

四次调用**全部**在右下角出现「AI生成」水印，包括提示词中明确写了 `no watermark`、`Avoid: ... signature, border, collage` 的第 2、3、4 段。结论：提示词层面无法关闭该水印。

---

# 第二轮：色域由场景决定

用户反馈「颜色不对，他是根据不同的照片风格来调整色彩风格的」。据此把色域从固定默认改为按场景选，并实测三个新色域验证。

## 5. 冷蓝夜渡（新增，通过）

输入角色：图 1 = 参考中的冷蓝渔舟（色域、表面）。输出：`../skills/dark-canvas/assets/calibrated-dusk-blue.jpg`。

```text
Create one original 3:2 fine-art image: a quiet oil painting on woven linen canvas, a dusk fishing scene.

Do not copy the reference scene. Build a new one.

Palette driven by the scene: deep cool blue-teal twilight, slate blue water, muted blue-gray sky. Low saturation throughout. One small restrained warm accent only: an orange-red life ring on the boat and a faint warm lamp glow, small and localized, nothing else warm. Deep near-black boat hull and figures.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than outline. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a digital grid.

Content and composition: a small wooden fishing boat with a simple canopy moored near the right bank, two small figures in pale shirts seated inside, seen at a distance. Reeds and a low dark bank frame the left edge. Open water fills the middle, a low hazy far shore behind. Sky fills roughly two thirds. Everything soft and atmospheric except the boat, which carries the single point of focus. Asymmetric, unhurried, generous empty space, quiet and solitary mood.

Avoid: warm golden sky, orange sunset, teal-orange grading, vivid saturation, HDR contrast, glossy photo look, thick impasto, text, signature, border, collage.
```

**结果**：冷蓝色域成立，**仅救生圈一处暖色**，织纹与油画感达标。右下角仍有水印。

## 6. 清晨薄雾（新增，通过）

输入角色：图 1 = 参考中的晨雾湖（色域、表面）。输出：`../skills/dark-canvas/assets/calibrated-morning-cream.jpg`。

```text
Create one original 3:2 fine-art image: a quiet oil painting on woven linen canvas, an early morning lake scene with wooded hills.

Do not copy the reference scene. Build a new one.

Palette driven by the scene: soft warm cream and pale gold light in the sky, hazy warm gray clouds, muted natural olive and deep green foliage on the hills, a cool gray-green water surface. Low saturation, gentle and restrained, nothing vivid. Deep near-black accents only in the closest foreground vegetation.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value rather than outline. Matte, no gloss, no varnish. Not a glossy digital photo, not thick raised impasto, not coarse burlap, not a digital grid.

Content and composition: a wide calm lake, a small wooden boat with a pale canopy near the left bank, a few tiny indistinct figures aboard. Forested hills recede behind in overlapping layers, each paler and softer than the one in front, fading into morning haze. A cluster of dark reeds enters the bottom right corner as natural framing. Sky fills roughly two thirds. One small flock of distant birds crosses the open sky. Asymmetric, unhurried, generous empty space, serene and solitary mood.

Avoid: vivid blue sky, orange sunset, teal-orange grading, oversaturated green, HDR contrast, glossy photo look, thick impasto, text, signature, border, collage.
```

**结果**：奶白暖光 + 灰绿林 + 远山退雾成立，母题（小船／鸟／芦苇）各一处未堆叠。右下角仍有水印。

## 7. 烟灰单色 · 重测（通过）

输入角色：图 1 = 参考中的单色月／枯枝（色域、表面）。输出：`../skills/dark-canvas/assets/calibrated-night-mono.jpg`。

```text
Create one original 3:2 fine-art image: a monochrome black and white oil painting on woven linen canvas, quiet and meditative.

Do not copy the reference scene. Build a new one.

Mood: hushed, still, solitary, a long silent evening. Nothing dramatic.

Medium and surface: oil paint on woven linen canvas. Clearly visible fine linen weave and fabric grain, continuous across the entire surface. Soft blended painterly tonal masses, gentle feathered edges, forms modelled by value instead of outline. Matte, no gloss. Not a glossy digital photograph, not thick raised impasto, not coarse burlap, not a repeating digital grid.

Palette: near-monochrome. Deep charcoal blacks, layered smoke-gray midtones, soft luminous pale gray in the sky. No color cast at all, no sepia, no warm tone. One small bright white disc high in the sky as the single point of light. The lightest area is a soft halo around it, fading outward into gray.

Composition: 3:2 landscape, low horizon. Sky fills roughly two thirds. A cluster of thin bare branches rises from the bottom edge, slightly left of center, with a second smaller cluster at the right. One small bright disc sits in the upper middle, clear of the branches. Generous empty space, asymmetric, unhurried.

Avoid: color, sepia, golden sunburst, central spotlight, epic cinematic landscape, HDR contrast, uniform global blur, thick impasto, text, signature, border, collage.
```

**结果**：纯黑白无色偏，月为唯一锐利处。右下角仍有水印。

## 水印专项测试

针对「能不能把水印去掉」做了专门尝试：

| 尝试 | 结果 |
| --- | --- |
| 提示词写 `no watermark` / `Avoid: signature` | 无效，7/7 复现 |
| 传 `footnote: ""` | **无效**，仍出现（该参数是水印文字，非开关） |
| 裁切底部 | **未采用**——属工具 AI 生成合规标识 |

**结论：水印在工具层与提示词层均无法关闭。** 处置：保留并说明，不擦除。

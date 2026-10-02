# 本次实际调用的提示词

工具：内建 image_gen；日期：2026-10-02。以下是调用时的完整文本。参考路径改写为公开仓库相对路径；执行时使用本机原始 PNG，公开参考 JPEG 与其画面相同。

## 从零生成

此测试使用旧 Creative OS 暖灰案例，在清晰摄影参考到达前执行，不代表修订后的默认配方。

输入顺序：已有风景案例（色调与表面）；已有植物案例（剪影与留白）。输出：`generate-cloud-bird.png`。

```text
Create one original landscape-format fine-art photographic image, approximately 3:2. A small dark bird gliding high over an irregular line of willow trees on a lake bank, viewed upward; sky occupies 70 percent, trees enter from the lower right and left edges leaving the center open. Physical look: darkroom photographic print fused into finely woven linen, visible tiny irregular warp/weft fibers across sky AND silhouettes, warm smoke gray / muted olive / parchment highlights with deep charcoal silhouettes. Brooding diffuse cloud banks with luminous cloud openings, compressed midtones, softly halated light, no bright blue, no orange sunset. Photographic observed nature with a haunting quiet unresolved mood, soft atmospheric depth; foliage still readable at selected edges, never an oil painting. Dense but fine textile texture—not coarse burlap, not regular digital pixel grid. Asymmetric open framing, no title, no watermark, no ornate borders, no collage, no signature. This is a completely new scene. Match the dark, low-saturation woven photographic surface and tonal restraint of the supplied style references; don't reproduce their scene or subjects' exact arrangement.
```

## 转换测试的合成输入

无参考图。输出：`transfer-source.png`。此图是 AI 生成的普通照片式输入，不是真实拍摄照片。

```text
Generate one ordinary realistic color photograph, landscape 3:2: a modest white rectangular wooden boathouse with a dark gray pitched roof on the right bank of a calm lake, a simple wooden dock extends from lower right toward the middle, one small red rowing boat tied to the dock, a leafy tree enters from the left edge, low hills across the far lake, sky occupies the upper half. Bright overcast afternoon, natural green foliage, soft blue-gray water and sky, ungraded clean digital camera photo, realistic detail and perspective, no print texture, no linen, no grain effect, no vignette, no paintings, no text, no people, no birds. This is an AI-generated test input photograph for a later image style-transfer experiment.
```

## 照片式图像转换

此测试也是 Creative OS 暖灰变体，发现较强的天空重绘偏差。中性灰转换另见下方。

输入顺序：`transfer-source.png`（编辑目标）；已有风景案例（色调与表面）；已有植物案例（剪影与表面）。输出：`transfer-dark-canvas.png`。

```text
Edit image 1, the source photograph. Image 2 is the tonal/surface style reference and image 3 is the botanical silhouette/surface style reference, not scene content. Preserve image 1's 3:2 crop, perspective, horizon, object count, and major positions: leafy tree on left, white wooden pitched-roof boathouse at right partly cropped, its doorway and window, diagonal wooden dock extending from lower right toward center, the ONE small rowing boat just left of the dock, rocks below the boathouse, hills across the lake. No new birds, kites, buildings, clouds-as-objects or extra boats. Transform rendering and surface only. Apply low-saturation smoke-gray, subdued gray olive and warm parchment, deep but differentiated charcoal foliage shadows, smoky layered midtones and soft restrained warm-gray sky highlights. Boat red becomes a small subdued oxidized-earth color, not a vivid accent. House walls remain relatively lighter but toned down. Add fine irregular linen warp/weft texture continuously over all areas, as though a darkroom photographic print has soaked into matte fabric, matching reference images 2 and 3; fine fibers not coarse burlap or digital grid. Keep photographic structure and recognizable dock, boat, roof, door and window edges. Soften distant hills and cloud edges slightly, retain important geometry. Preserve all scene content, no global blur, no thick paint or brushstrokes, no text, no watermark, no borders, no collage. The result should visibly belong to the same subdued dark textile photographic family as references 2 and 3 while still being the SAME source scene.
```

## 中性灰校准生成

输入顺序：用户清晰阴云飞鸟参考（色调、表面）；用户清晰枝叶参考（剪影、细纹）。第三方参考文件仅保存在本地，不随公开仓库分发。输出：`../skills/dark-canvas/assets/calibrated-neutral.png`。

```text
Generate a new original 3:2 photograph-style image. Use image 1 only as the reference for neutral gray tonality, cloudy light, fine flat print surface and restrained edge wear. Use image 2 only as the reference for natural dark foliage edges and the subtle fine surface texture. Do not reproduce either reference composition. New scene: looking upward across a quiet rural valley, uneven distant tree silhouettes occupy only a narrow bottom band, a close sparse leaf branch enters the top right, one very small distant bird in the left third of the open sky. Mostly sky, natural irregular overcast cloud layers, pale diffuse silver-gray top sky gradually deepening to charcoal cloud at lower right, no golden sunburst or central dramatic spotlight. Neutral monochrome with only a trace of warm gray, truly black silhouettes against lighter sky; photographic tonal gradients and restrained softness. Closely match the reference's fine flat softly visible crosshatched print surface: tiny evenly distributed fiber/dot-like marks, no raised threads, no heavy canvas or burlap, no painterly marks, texture must be quieter than the imagery and uninterrupted across the frame. Very faint irregular print wear near extreme edges, no drawn frame or heavy vignette. A candid atmospheric photographic observation, simple unresolved framing, not an epic fantasy landscape, not a painting. No warm sepia or amber grading, no orange leak, no added objects, no text, no signature, no watermark, no collage.
```

## 中性灰转换

输入顺序：`transfer-source.png`（编辑目标）；用户清晰阴云飞鸟参考（色调、表面）；用户清晰枝叶参考（剪影、细纹）。输出：`transfer-neutral.png`。

```text
Edit image 1, the source photograph. Images 2 and 3 are tonal and surface style references only. Keep the exact source framing, scene, camera position, crop and perspective: leafy tree entering from left, white wooden boathouse with pitched roof and a doorway plus one visible window on right, diagonal dock from lower right to middle, exactly one small boat at the dock, rocks along the bank and layered distant hills. Preserve the original cloud layout and diffuse overcast lighting; do not add a sunburst, central light beam or new dramatic cloud structures. Match reference 2's neutral monochrome smoke-gray tonality with only an extremely slight warm-gray tint, pale silvery sky gradients, darker soft distant hills, deep nearly black foreground foliage and shadows. Preserve readable roof, door, window, boat outline, dock posts and planks, without crisp HDR. Match reference 2 and 3's very fine flat subdued photographic-print crosshatch texture, tiny softly visible fiber/dot-like marks continuous over the whole photograph, no raised linen threads, no heavy burlap or warm sepia. Light irregular print wear at extreme edges is acceptable but no drawn border. Boat becomes subdued dark gray; retain its position and structure. The surface and tonal rendering change; all source objects remain in place and identifiable. No added birds, kites or other objects, no painterly strokes, no global blur, no text, watermark or signature.
```

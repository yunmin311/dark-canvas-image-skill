# v0.5.0 完整实际提示词

图片均为内建 image_gen 调用，transparent_background=false。调用中只使用 prompt 和真实本地 referenced_image_paths；以下将私有绝对路径改写为角色名。完整私有记录位于本地 test-spec.json。

## 调用 1 · lake

输入顺序：用户湖面原图；用户枝叶作品参考（仅笔意/色面）；技能内 rough-linen-ao-1k.jpg（仅经纬形态）。

```text
Edit image1 only. Image1 supplies all colors, light level, willow/lake subject and 4:3 composition. Preserve its warm-neutral gray sky, near-black green willow and tree mass, dark gray lake, tiny original warm and cyan lights. Do not turn it blue, beige, rose or orange; only a small exposure lift is allowed. Image2 supplies Chinese brush-painting-like economy: quiet unified background tone and simple dark tapered brush forms, NOT its colors, bird or scene. Image3 is a REAL linen weave reference; borrow fine straight warp/weft structure only, not its white background or strong contrast. Recast existing foliage and reflections into economical ink-brush-like shapes on primed oil canvas, opaque subdued pigment and faint dry-brush drag at a few edges. Keep open sky/water as continuous uniform tonal fields with very restrained gradients. Suppress individual leaf, glare and camera sharpness. Fine weave integrated into pigment, visible but quiet. No watercolor blooms, watery paper staining, ornate curls, decorative scratched loops, coarse burlap or thick impasto. No added bird, boat, moon, object or text. Deliver one finished calm Chinese-brush-inspired canvas picture with source colors preserved.
```

## 调用 2 · stilllife

输入顺序：已有 AI 静物原图 examples/adaptive/stilllife-v1.png；用户枝叶作品参考（仅笔意/色面）；技能内 rough-linen-ao-1k.jpg（仅经纬形态）。

```text
Edit image1 only, retaining its exact square crop, one brick-red mug with one handle, one ivory saucer and one spoon in the existing arrangement. Keep its original brick-red, ivory and dark warm-brown palette and relative color proportions; no rose wash, orange recoloring, whitening or blanket desaturation. Image2 is ONLY a reference for unified quiet background tone and Chinese brush-painting-like economical forms, not its bird/branches/sepia color. Image3 is real linen weave: borrow fine straight warp/weft morphology at low contrast, not its white color. Render the objects with confident simple ink-brush-like pigment shapes on primed oil canvas; some edges may retain tapered dry-brush traces. Unify wall/table within their original color families, reduce woodgrain, glossy highlights and photographic microdetail. Flat quiet opaque pigment, material tooth from actual linen, calm continuous background color. Not watercolor on paper: no translucent blooms, stained rims or paper flecks. No curly etching, ornamental embossing, coarse weave, impasto, extra props or text. Deliver the final Chinese-brush-inspired quiet canvas still life without substantial color changes.
```

## 调用 3 · stilllife

输入顺序：本轮 stilllife-v1.png；用户枝叶作品参考（仅笔意/色面）。

```text
Edit image1. Its brick-red, ivory and warm-brown colors, canvas weave, exact square composition and one mug/handle/saucer/spoon are already correct; keep them. Correct the overly busy Western-oil-paint handling: remove white scratched knife-like dabs, jagged scattered paint marks and fussy woodgrain. Use image2 ONLY for economical Chinese brush-painting-like shapes and a quiet unified field, not its palette or subjects. Cup, saucer and spoon should become calm flat color forms with a few tapered brush-edge traces; retain their basic shapes, avoid modeling every shiny highlight. Background/table remain their original dark warm-brown, now much more uniform and tranquil. Keep existing fine straight linen weave everywhere without amplifying it. No hue shift, rose/orange wash, paper/watercolor bloom, blur, new objects, text or border. Deliver the completed restrained Chinese-brush-like still life on canvas.
```

## 调用 4 · stilllife-v3

输入顺序：本轮 stilllife-v2.png；用户枝叶作品参考（仅笔意/色面）；技能内 rough-linen-ao-1k.jpg（仅经纬形态）。

```text
Edit image1 into a quiet Chinese brush painting on fine linen. Keep the exact square crop, arrangement, one brick-red mug/handle, one ivory saucer, one spoon, warm brown table/wall and pale window. Keep these source colors. Image2 provides ONLY economical tapered Chinese brush shapes and quiet continuous background fields. Image3 supplies ONLY the fine straight horizontal/vertical linen structure. The key correction: flatten the mug, saucer and spoon into broad simple opaque color silhouettes, greatly reducing rounded 3D modeling, cast-shadow contrast and shiny white highlights. The mug is mostly one calm brick-red color shape, dark drink a simple flat oval; handle a tapered red brush loop. Saucer one restrained ivory brush form, spoon a few quiet gray-beige strokes. A few meaningful brush starts and tapered ends, no busy paint scratches. Background and table broad uninterrupted warm-brown fields. Replace all curly vermicular engraving with subtle regular straight linen weave integrated into pigment, faint and fine everywhere. The entire result should have the economical brush feeling of Chinese landscape painting applied to this still life, with suppressed volume and quiet color fields. No watercolor transparency, stained paper, mottled wash, thick impasto, ornate texture, hue changes, extra objects, text or border.
```

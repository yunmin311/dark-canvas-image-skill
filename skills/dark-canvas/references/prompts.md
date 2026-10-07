# 图生图请求模板

先保留源照片曝光、光向与主色，再指定默认经纬画布；七组只决定本次主体取舍与局部效果。田野农人不使用，灰湖颗粒不作为默认。下面是请求内容，不是图像工具的新参数。按本次选择替换括号，只保留需要的表达；不要把选项全部写进同一张图。源图已给定时不用新建合成场景。

## 基本编辑

先用简短请求，实际附入原照片和选定作品，不用作者名代替作品：

```text
Translate [main subject] in image 1 into the same finished-image relationship visible in image 2: [thin shapes/contour behavior], [continuous ground tones], and [visible canvas and wear relationship]. Keep [source exposure, shadow depth, existing light direction, color families, subject placement and crop]. Let [secondary elements] disappear into the ground. Shapes and surface should form one completed image. Do not borrow image 2's subjects or palette. [One observed failure to correct, if needed.]
```

需要进一步区分角色/区域时再使用以下展开版本；不能把所有可选短句堆进去。

```text
Edit image 1. Preserve its original exposure and existing light relationships; let the weave take each region’s source color instead of lifting its brightness. Keep [main subject and its recognizable silhouette/gesture], [user-required counts or details], original crop and source palette: [main color relationships]. Simplify, merge or omit [secondary elements] so they no longer compete with the subject. Consolidate small source colors within their original families.
Image 2 is the artwork reference for [chosen form/edge treatment], [surface/wear] and [vignette level], not for its subject, composition or palette.
[If needed: Image 3 is the selected material reference for weave/wear morphology only, not its gray color or contrast.]
Apply [retained photographic shapes / economical Chinese-brush-like handling / clean flat cut-paper-like silhouettes / selective directional softening] to [regions]. Match the reference's quiet background and unified tonal fields. [Chosen canvas/wear treatment.] [Chosen vignette treatment, or none.]
Preserve natural irregularity and subject-defining details; allow secondary detail to disappear. Establish quiet planar shapes before surface effects. Do not invent props, change the crop, globally recolor, add glossy 3D modeling, ornate texture or a theatrical antique frame. Do not introduce paper layers or paper grain merely because silhouettes are cut-paper-like. Deliver one finished poetic image.
```

## 可选表达短句

- 毛笔：`Economical directional forms with tapered endings, a few restrained dry-brush edges; no scattered oil-paint dabs or modeled shiny highlights.`
- 剪影：`Keep recognizable crisp silhouettes and meaningful small branches; simplify internal shading into calm flat dark forms. No layered paper sculpture or added paper material.`
- 保留摄影色形：只在当前作品及用户目标允许时使用 `Keep naturally irregular source contours and subject-defining details; reduce internal modeling so shapes belong to the same matte surface.` 用户要手绘感时，不追加要求全图仍像照片的限制。
- 雾化/拖影：`Keep selective softening in [region/direction], while [recognition-critical shape] stays readable. Not uniform blur.`
- 动态人物：`Keep posture, placement and broad clothing color shapes. Merge folds, markings and equipment detail; soften the figure pigment with restrained directional smearing and faint overlapping impressions, as in the actual motion reference. Keep the canvas weave itself stable and readable. No additional people or duplicated limbs.` 按图选择方向与程度，不能给所有人物自动套用。
- 舟上人物（R12）：`Treat person, action, hull and boat shadow as one softly overlapping pigment group: human in broad clothing/head shapes, boat in a long dark shape. Merge face, clothing, equipment and hull fine detail; apply selective softening/light overlap across this group while the canvas remains stable. Keep source posture, subject count, placement and exposure.` 不另加“船和倒影不动”的冲突限制，不能用清楚船体衬一团糊人。
- 细布：`Match the reference's visible woven pitch and contrast through both ground and subject, with thin flat color shapes on the same surface.` 不默认写成 barely visible，也不强行使用粗布。
- 局部旧痕：`Sparse uneven old staining, a few rubbed thin spots and isolated small scuffs, with large continuous quiet areas. No uniform dirt overlay.`
- 磨损残破：`Localized pigment losses, tiny exposed-ground flecks and a few irregular scratches, matched to the artwork's scale; intact continuous cloth remains. No large holes, burn edges, decorative crackle or plaster chips.`
- 晕影：`[Subtle/visible] broad soft edge falloff matching the artwork, within source colors, no hard black corners or border; preserve the original crop.`
- 无晕影/无做旧：必要时写明 `Keep edges open; no added vignette.` / `Clean cloth surface; no added age marks.`，不默认给每张加入这些限制。

## 用户指定候选之间中和

复杂公园的分步色块路线已被用户否定，不继续把“先色块再布面”作为推荐。用户认为 direct 版还可以，并指定与旧稿取中间表达时，按明确属性修改，不作像素平均叠加：

```text
Edit image 1, the selected candidate. Keep [its natural contours, quiet thin pigment and surface]. Borrow a moderate amount of [specific readable forms or tonal variation] from image 2, without restoring [rejected detail or effects]. Image 3 is the original source for layout and light relationships. Keep the established exposure and restrained palette; do not add further grading or texture. Deliver a natural middle treatment, not doubled contours, vector blocks or a literal pixel blend.
```

候选角色、用户最新选择和取舍属性都要记录。旧稿被指定作局部比较依据，不等于其整体已通过。

## 定向修正请求

```text
Correct only [observed problem] in this candidate, using the original source again where content or colors drifted. Preserve [already correct content/color/form/material]. Match [chosen reference property] in [region]. Keep [wear/vignette] only at its selected level; do not change other style choices. No new props or crop changes.
```

修正必须来自实际看图，不能因换了模板就记为通过。失败候选有明显配色或材质漂移时，不再把它当额外图像参考反复传入；重新附源图和正确作品，在文字里指出偏差，避免错误外观成为新的锚点。完整实际请求、输入顺序、输出路径与每轮观察保存到任务记录；未出图不写成“已验证”。

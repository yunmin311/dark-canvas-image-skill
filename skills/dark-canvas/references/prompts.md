# 为本次目标组装提示词

模板的方括号必须按实际看图替换；不适用的条目删除。它们是生成结构，不是已通过所有主题的固定成品配方。工具参数以当前接口为准。

## 新图

```text
Create one original [requested aspect ratio / format] image for [purpose].
Subject and scene: [specific requested content and object/person counts].
Composition: [appropriate framing for this subject; honor the requested crop and focal content].
Input references: image 1 = [palette and contrast only]; image 2 = [surface / edge treatment only, if needed]. Borrow these visual properties, not their subjects, scene geometry or object placement.
Visual treatment: a quiet flat painting on fine canvas with [continuous delicate linen weave and thin matte pigment / another user-selected treatment]. [soft integrated edges and simplified pigment shapes; only retain explicitly needed recognition cues]. Mood and lighting: [selected from the request and current references].
Poetic intent: [one subject-specific emotional relationship]. Express it through [tonal unity, quiet color fields, lost edges and restrained detail]. Avoid competing spectacle; keep requested subjects/counts intact. Strong depth, clear layers and photographic sharpness are not quality goals. The subject itself must participate in painterly abstraction.
Palette: [target temperature, dominant color relationships and any important local color]. Surface scale and intensity: [observed reference level]. Keep main subject arrangement; allow fine details, material rendering and reflections to dissolve into quiet thin pigment. Delicate brush handling is allowed; avoid thick impasto or coarse weave.
Must include/retain: [critical content]. Do not add: [reference-only motifs irrelevant to the task].
Avoid: [only relevant failure risks, such as all-over sepia, coarse burlap, ornamental etched texture, or loss of explicitly requested subject features]. No unrequested text, decorative frame, signature or collage.
```

## 照片转换

```text
Edit image 1, the source. Other images are style references only.
Keep image 1's [actual aspect ratio], crop, camera position, main scene arrangement. Preserve [actually observed people, objects, counts, main shapes and positions; only preserve fine details when explicitly required].
Change [authorized rendering/palette/surface/softness]. Palette target: [chosen reference or explicit request; do not force warm or gray onto every scene]. Surface target: [observed scale and flatness]. Compress strong spatial/tonal separation; soften and simplify foreground as well as background into integrated pigment shapes. Keep only [explicit task-critical recognition cues].
Do not insert [objects appearing only in the references]. Do not delete content or alter framing to create negative space. Preserve [sky/cloud layout, reflections, lettering or identity, if required], and avoid [observed likely drift].
Poetic intent: [a relationship already present in the source, such as suspended willow lines and still water]. Express it through a unified calm picture plane, subdued tones and thin paint in fine linen weave. Do not strengthen perspective, layers or sharpness as default improvements.
The same source scene must remain recognizable. Allow painterly detail abstraction. No extra motifs, uniform out-of-focus blur, dramatic depth, thick impasto, coarse burlap, borders, text or signature.
```

## 定向修正

```text
[Edit the best prior result OR regenerate from the original source and references, whichever preserves content better].
Observed failure: [concrete visible mismatch]. Correct only [targeted property].
Keep [successful content, framing and treatment]. Invariants: [list critical retained facts again].
Use [specific reference] for [specific property]. Do not repeat [observed failure].
```

工具强制标识只能根据本次输出和宿主说明记录；提示词不能保证删除、关闭或一定出现某个水印。所有最终提示词、参考角色、修正和实际输出需进入任务记录。

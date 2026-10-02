# 可执行提示词

将方括号替换为本次要求。删除不适用的语句；不要把所有变体塞进一次调用。固定提示词不保证固定结果。

## 从零生成

```text
Create one original [aspect ratio] fine-art photographic image of [requested subject and scene].
Style references: image 1 = surface and tonal reference; image 2 = silhouette/negative-space reference. Use their visual language, not their exact scenes.
Composition: [user composition; otherwise asymmetric framing, broad quiet sky or mist, peripheral natural silhouettes, one small focal anchor only when suitable].
Photographic space and believable organic shapes, with fine flat photographic print texture: tiny softly visible crosshatched fibers or dot-like marks continuous through light and dark areas, matte, no raised threads. [For the Creative OS variant only: a more visible fine linen weave]. Not coarse burlap or oil-paint brushwork.
Palette: [default neutral monochrome smoke-gray with a trace of warm gray; otherwise muted olive / warm parchment OR restrained ochre / brown-black]. Truly dark silhouette masses, layered gray midtones, softly diffuse lighter sky; subdued saturation, atmospheric depth. Selectively readable edges with softly fading distance. No central golden sunburst or epic cinematic landscape unless requested.
Optional variant: [local directional motion blur OR a restrained edge light leak; omit by default].
No text, watermark, signature, decorative border or collage. Avoid vivid blue skies, orange-teal grading, HDR crispness, thick paint, pixel grids and uniform blur.
```

## 将照片转换为暗幕质感

```text
Edit image 1, the source photograph. Images 2 and 3 are style references only.
Preserve the source's aspect ratio, crop, perspective, horizon, subject identities, object count and major positions. Specifically preserve [list actual landmarks/people/objects after viewing the source]. Do not borrow or insert objects from the style references.
Transform tonal rendering and print surface to match the reference: low-saturation [default neutral smoke-gray; otherwise chosen palette], deep but differentiated charcoal shadows, layered smoky midtones and soft gray highlights. Add fine flat softly visible crosshatched fiber/dot-like print texture continuously across the photographic image. [Only for the Creative OS variant: fine linen warp/weft texture, as though the print has soaked into a matte fabric surface]. Keep texture small and subtle, never coarse burlap or a digital grid. Do not add a golden central spotlight or reshape clouds dramatically.
Maintain photographic structure and recognisable important edges. Soften only [source-appropriate background areas]; keep [faces, buildings, foreground landmarks] readable. [Motion/edge leak only if explicitly selected].
Change the photographic rendering and surface; retain the scene. No new text, objects, signature, watermark, decorative border or collage. Avoid oil-paint brushwork, uniform sepia, crushed full-frame blacks, oversaturation and global blur.
```

## 交付记录

写出：最终提示词、每张输入的角色、生成/编辑工具、输出路径、对照参考的可见偏差。隐私路径可以保留在本地记录；公开记录使用仓库相对路径，不放分享令牌或个人文件夹地址。

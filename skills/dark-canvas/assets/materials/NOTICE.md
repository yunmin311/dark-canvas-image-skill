# 表面素材的选择与来源

| 文件 | 性质与来源 | 什么时候用 |
| --- | --- | --- |
| [rough-linen-ao-1k.jpg](rough-linen-ao-1k.jpg) | 实际亚麻灰度遮蔽贴图，Poly Haven CC0，原文件未改 | 细经纬的形态依据；干净布面，或做旧前的织物基底 |
| [rough-linen-disp-1k.jpg](rough-linen-disp-1k.jpg) | 同一材质的原始高度图，CC0 | 辅助辨认纤维方向，不是最终图片的灰度底色 |
| [worn-canvas-guide.png](worn-canvas-guide.png) | 内建 image_gen 编辑真实亚麻得到的生成示意 | 轻旧色斑、磨薄与少量擦痕；不是实拍旧画布 |
| [distressed-canvas-guide.png](distressed-canvas-guide.png) | 同上，修正后选择的生成示意；借用户作品表面旧痕的尺度关系 | 更明显的局部旧斑、露底/颜料缺口与细擦痕；不是摄影师原素材 |

两张生成片是形态参考，不是完全匹配参考作品的保证。它们的灰色、原贴图对比与纤维密度不能直接套到照片上。**成图的织纹尺度/强度、磨损密度以当前作品为准**，借结构和不均匀性，保留源图颜色；无需再修材质时，直接原图 + 作品参考即可，不强制多附贴图。

做旧程度分别选择：干净 / 轻微 / 明显。生成片里露出的纤维仍较多，不能把成图变成裸麻布。选了旧痕时保留有意的磨损，不把它全部去噪；没选旧痕就不加脏斑。不要用破洞、烧边、裂纹网、石膏剥落或复古画框解释每张图的残破感。晕影是另一项边缘处理，不是这些布料本身必须携带的黑框。

优先原作共同布面。这些素材只在需要额外校准时辅助，不作为覆盖原曝光和色彩的默认底图；先读 [画布与光色](../../references/canvas-and-light.md)。

## 原始亚麻来源

[Poly Haven Rough Linen](https://polyhaven.com/a/rough_linen)，摄影 colormass，处理 Rico Cilliers。[官方 CC0 许可](https://polyhaven.com/license)；素材保留 CC0，不改成项目文字的 MIT 许可。下载 URL、字节数、SHA256 与日期见 [provenance.json](provenance.json)。这是亚麻织纹资源，不证明与摄影师底布同款或是已上底油画布实拍。

## 生成示意来源

2026-10-03 Codex 内建 image_gen 三次实际编辑，两张初稿加一次明显磨损修正。输入为上述 CC0 亚麻；修正时另附用户黑白枯枝月作品，只借表面旧痕的尺度/不均匀性，不复制树、月、场景或具体旧痕位置。第三方作品不随包分发。生成示意不是 CC0 实拍资源，不能伪装成摄影师素材；原始 PNG 未作后期编辑。完整实际请求见 [generated-prompts.md](generated-prompts.md)，尺寸、校验与选择原因见 [generated-guides.json](generated-guides.json)。

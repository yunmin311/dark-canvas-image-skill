# 图片来源与范围

| 文件 | 来源 | 用途 |
| --- | --- | --- |
| skills/dark-canvas/assets/calibrated-ochre-canvas.jpg | 2026-10-02 内建 `image_gen`，按默认暖金亚麻配方生成 | **默认配方校准样本** |
| skills/dark-canvas/assets/calibrated-monochrome.jpg | 同日 `image_gen`，烟灰单色变体 | 单色变体校准 |
| skills/dark-canvas/assets/calibrated-neutral.jpg | 上一轮 `image_gen`，旧中性灰配方 | **仅作对照**，非推荐输出 |
| skills/dark-canvas/assets/accepted-landscape.jpg | 用户已有 Creative OS AI 生成案例的 JPEG 版本 | 校准灰褐风景、层次与表面 |
| skills/dark-canvas/assets/accepted-botanical.jpg | 用户已有 Creative OS AI 生成案例的 JPEG 版本 | 校准植物剪影、暖灰色域与留白 |
| examples/transfer-canvas.jpg | 2026-10-02 `image_gen` 编辑 `transfer-source.jpg` | 亚麻油画转换实测 |
| examples/transfer-source.jpg | 上一轮 `image_gen`，AI 合成普通照片式输入 | 转换输入，非真实拍摄照片 |
| examples/legacy-neutral-recipe.jpg | 2026-10-02 `image_gen`，复现旧中性灰配方 | 旧配方对照 |
| examples/generate-cloud-bird.jpg | 上一轮 `image_gen`，旧暖灰从零生成 | 历史对照，场景有偏差 |
| examples/transfer-dark-canvas.jpg | 上一轮 `image_gen` 转换 | 历史对照，天空重绘偏差 |
| examples/transfer-neutral.jpg | 上一轮 `image_gen` 转换 | 历史对照，云形重绘偏差 |

以上均为用户授权公开范围内的 AI 生成示例，**不是摄影师的摄影作品**。MIT 许可证适用于本仓库的原创文字与配置，不表示第三方摄影作品被重新许可。

用户提供的第三方摄影参考保存在被 Git 忽略的本地目录，不随仓库与发布包分发。原始 Creative OS 文件未被改动。

**已知工具缺陷**：内建 `image_gen` 在所有输出右下角自动压印「AI生成」水印，提示词无法关闭。这些示例图的水印**未做后期移除**，保持工具原始输出以供核验。

所有示例图以 JPEG（quality 88）保存，由工具原始 PNG 无损转色而来，仅为压缩体积（合计约 3.1 MB）；画面内容、构图与水印均未改动。

# 图片来源与范围

全部图片均为 AI 生成的校准样本，**不是摄影师 Pablo Bueno 的摄影作品**。

| 文件 | 来源 | 用途 |
| --- | --- | --- |
| skills/dark-canvas/assets/calibrated-ochre-canvas.jpg | 2026-10-02 `image_gen`，暖金夕照色域 | 色域校准：暖金 |
| skills/dark-canvas/assets/calibrated-dusk-blue.jpg | 同日 `image_gen`，冷蓝夜渡色域 | 色域校准：冷色 + 单一暖色锚点 |
| skills/dark-canvas/assets/calibrated-morning-cream.jpg | 同日 `image_gen`，清晨薄雾色域 | 色域校准：奶白暖光 + 灰绿 |
| skills/dark-canvas/assets/calibrated-night-mono.jpg | 同日 `image_gen`，烟灰单色色域 | 色域校准：纯黑白 |
| skills/dark-canvas/assets/calibrated-neutral.jpg | 上一轮 `image_gen`，旧中性灰配方 | **仅作对照**，非推荐输出 |
| skills/dark-canvas/assets/calibrated-monochrome.jpg | 上一轮 `image_gen`，烟灰单色变体 | 历史对照（已被 night-mono 取代） |
| skills/dark-canvas/assets/accepted-landscape.jpg | 用户已有 Creative OS AI 生成案例 | 校准层次与表面 |
| skills/dark-canvas/assets/accepted-botanical.jpg | 用户已有 Creative OS AI 生成案例 | 校准植物剪影与留白 |
| examples/transfer-canvas.jpg | 2026-10-02 `image_gen` 编辑 `transfer-source.jpg` | 亚麻油画转换实测 |
| examples/transfer-source.jpg | 上一轮 `image_gen`，AI 合成普通照片式输入 | 转换输入，**非真实拍摄照片** |
| examples/legacy-neutral-recipe.jpg | 2026-10-02 `image_gen`，复现旧中性灰配方 | 旧配方对照 |
| examples/generate-cloud-bird.jpg | 上一轮 `image_gen`，旧暖灰从零生成 | 历史对照，场景有偏差 |
| examples/transfer-dark-canvas.jpg | 上一轮 `image_gen` 转换 | 历史对照，天空重绘偏差 |
| examples/transfer-neutral.jpg | 上一轮 `image_gen` 转换 | 历史对照，云形重绘偏差 |

## 权利说明

MIT 许可证适用于本仓库的原创文字与配置。**不表示第三方摄影作品被重新许可。** 仓库内所有图片都是 AI 生成的原创样本，未复制、未裁切自摄影师的任何一张作品。

用户提供的摄影参考保存在被 Git 忽略的本地目录，**不随仓库与发布包分发**。小红书分享链接的临时参数（`xsec_token`、`shareRedId` 等）已全部剔除，只保留稳定主页地址。原始 Creative OS 文件未被改动。

## AI 生成水印

内建 `image_gen` 在所有输出右下角自动压印「AI生成」水印，**7/7 次实测复现**，提示词与 `footnote` 参数均无法关闭。

该水印是工具对 AI 生成内容的**合规标识**，本仓库**予以保留、不做擦除**，包括用于展示的全部示例图。若需要无水印版本，只能更换不带水印的图像服务（工具选型变更）。

所有示例图以 JPEG（quality 88）保存，由工具原始 PNG 转换而来，仅为压缩体积；画面内容、构图与水印均未改动。

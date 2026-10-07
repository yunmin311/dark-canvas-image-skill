# 当前验收记录 · Current validation status

更新：2026-10-07。记录用户对具体输入与版本的选择，不等于整类题材都能稳定复现。用户验收优先于 AI 自评；新修订的文字尚未重新进行独立出图回归。

Updated 2026-10-07. Approval applies to specific inputs and selected outputs, not whole subject categories. User acceptance takes precedence over model self-assessment. The documentation changes have not undergone a new independent image-generation regression.

## 已通过的具体案例

以下路径相对于本地 `local-reference/tests/`，便于核对；照片和测试结果不随公开包分发。公开安装环境可使用用户附图或两张已认可的 Creative OS AI 案例，不能声称已看过缺失的作品。

| 题材 | 用户选定版本或范围 | 可复用的处理依据 |
| --- | --- | --- |
| 柳岸画布强度 | `2026-10-04-canvas-first/result-v1.png` | 第一版较克制；第二版偏强 |
| 荷叶灯影、柳枝双灯 | `2026-10-04-three-photos/` 前两张 | 保原夜景曝光，布面不靠提亮显露 |
| 竹叶近物、湖岸枯树 | `2026-10-05-matched-themes/`；枯树 v3 | 薄形与自然细线，次要细节合并 |
| 雾中人舟 | `2026-10-05-matched-themes/rowboat/result-v5.png` | 人衣、动作、船体与船影一起取舍；只糊人物的旧稿失败 |
| 柳岸雾山 | `2026-10-05-mist-shore/` 本轮 | 用户通过整轮，未指定 v1/v2 偏好 |
| 暖云近树、暗云亮缝 | `2026-10-05-cloud-rework/`；近树 v2、云带 v3 | 合并碎叶亮孔与凸起碎笔，保大云走势与原亮缝 |
| 雾中芦苇 | `2026-10-05-reeds-blossoms/reeds/result-v2.png` | 细枝与雾面相融，织纹稳定 |
| 亮底玉兰 | `2026-10-06-bright-large-subject/result-v2.png` | 部分瓣边与背景相融，避免逐瓣塑形；早期花稿认可已撤回 |
| 雾山乡村 | `2026-10-06-bird-village/village/result-v4.png` | 保树屋、坡面与果园关系，减少内部碎细节，不套水彩配色 |
| 彩鸟 | `2026-10-06-bird-village/bird/result-v6.png` | 收敛过强彩度，局部柔化；纠正第五稿整体压暗，不推广为所有图必须降饱和 |
| 秋叶 | `2026-10-06-leaves-coast/leaves/result-v2.png` | 用户选择中间稿，第三稿未被选定；保原透光暖色并融合次叶 |
| 雾海礁岸 | `2026-10-06-leaves-coast/coast/result-v4.png` | 保冷灰曝光、自然岩形与水道，减少微纹并选择性柔化远岩 |

## 未通过或待验证

复杂公园仍未通过。用户曾认可 direct 稿的部分表现并要求与旧稿中和，随后暂停该轮；这不是整张通过。不能将它作为正确风格参考。

尚无证据证明所有复杂建筑、密集景物、动物或人物都能稳定适配。七个作品观察分组只是选参考的依据。缺少原作的公开安装环境与私有参考库也不是相同的测试条件。

历史失败、暂存与撤回记录见 [主题适配](landscape-adaptation.md)；早期 v0.6.0 实测保留在仓库的 `examples/validation.md`。最新选择覆盖旧状态，不抹除失败过程。

## Release scope

The v0.7.0 package contains the current instructions, observation index, editing templates, this acceptance record, two approved Creative OS AI examples, and separately attributed material guides. It excludes private photographic references and test outputs. The seven reference groups are routing guidance; approval is per input and selected version. Complex park scenes remain unapproved, and behavior without the private reference library has not been established as equivalent.

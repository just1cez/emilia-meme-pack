# 爱蜜莉雅 Q版表情包

这是一个面向 AstrBot Meme Manager 的社区同人资源包，当前版本包含 **120 张透明 PNG**，覆盖 21 个语义分类和更多日常动作。

![表情包预览](previews/cover.png)

## 安装

在 AstrBot 表情包管理器的 WebUI 中打开**资源广场**，通过 GitHub 仓库地址安装：

`https://github.com/just1cez/emilia-meme-pack`

仓库分支为 `main`，包根目录为 `.`。安装后在**设置中心 → 使用规则**中将本包设为默认，或绑定到指定会话、人格。逐图语义检索还需配置语义模式与向量模型并建立索引。

## 目录

- `manifest.json`：资源包元数据与分类说明（版本 `0.4.1`）
- `memes/<category>/`：120 张透明 PNG 素材
- `previews/cover.png`：封面
- `previews/overview.png`：全量预览
- `memes_data.json`：分类说明兼容文件
- `source_index.json`：文件哈希与尺寸索引
- `semantic_metadata.json`：逐图 caption、tags 和语义索引

## 逐图语义说明（0.4.1）

120 张图片均附中文描述及动作、情绪、道具、聊天用途标签。描述首句记录可见画面，后句说明建议使用场景；图片身份仍由内容哈希、分类和相对路径共同确定。

本轮按实际图片纠正了文件名造成的歧义，例如 `comfort/0004_thumbs_up.png` 实际为双拳打气，`affection/0006_pat_received.png` 实际为幸福托腮。文件名与图片路径保留，检索应使用逐图描述与标签。

下载完整包后，用浏览器打开 [逐图语义浏览页](previews/semantic-review.html)，可按分类和关键词筛选图片、描述与标签，并查看相似动作说明。描述经过 Codex 逐图视觉核对；基础包与语义扩展已通过官方 Schema、文件路径、内容哈希和条目 ID 检查，尚未进行 AstrBot 实际安装、发送和向量检索测试。

张臂欢迎与拥抱、几张鼓掌等图像存在实际重叠，建议用途不能保证唯一选图。分类模式仍按类别选图；要使用逐图语义，需在插件中配置语义模式并建立索引。已有索引应在导入新描述后更新。

## 设计说明

角色统一采用银白长发、紫色眼睛、白紫服装、蓝绿色吊坠、圆脸大头和粗紫线条。动作扩充参考了聊天表情包中的庆祝、鼓掌、抗议、摸头、吃喝、工作、唱歌、跳舞、害羞、睡觉等常用语义，但所有图像均重新生成，没有直接复制参考仓库的图片。

本次动作语义参考：[seio-stickers v2026.09.0](https://github.com/anka-afk/seio-stickers/tree/v2026.09.0)、[congyu-meme-pack v1.0.0](https://github.com/anka-afk/congyu-meme-pack/tree/v1.0.0)、[deepseek-fanart-meme-pack v1.0.0](https://github.com/anka-afk/deepseek-fanart-meme-pack/tree/v1.0.0)，构图参考了[拉菲2表情包](https://github.com/anka-afk/laffey2-meme-pack)。角色识别参考[Re:ZERO 官方角色页](https://www.re-zero.com/character/%E3%82%A8%E3%83%9F%E3%83%AA%E3%82%A2/)和 [Good Smile Nendoroid Emilia](https://www.goodsmile.com/en/product/4070/Nendoroid%2BEmilia)。

## 版权与使用

爱蜜莉雅、Re:Zero 及相关角色形象属于原权利人。本包是非官方 AI 生成同人资源，仅建议个人非商业使用；发布或再分发前请自行确认当地法律和原作者/权利人的要求。

项目代码与元数据的 MIT 许可见 [LICENSE](LICENSE)。


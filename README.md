# zangyu-asr-models

藏文观修辅助器（https://www.tbmeditation.uk）「上传整段音频，自动切成单字」用的识别模型分片，经 jsDelivr 加速下载。

jsDelivr 的 GitHub 通道单文件上限 20MB、一个版本上限 150MB，所以模型切成 ≤ 19MB 的分片，按顺序分成几组，每组是一个 tag（只含这一组）：

| tag | 内容 |
|-----|------|
| `w2v-base-960h-int8-v1-a` | 标准模型 wav2vec2-base-960h int8 全部分片（Apache-2.0） |
| `mms-fa-int8-v1-a` / `-b` / `-c` | 高精度模型 MMS_FA int8 的三组分片（CC BY-NC 4.0，非商业使用） |

下载地址：`https://cdn.jsdelivr.net/gh/AriaYD/zangyu-asr-models@<tag>/<模型 id>/part-xx.bin`。
分片顺序、大小与 sha256 见网站的 `/models/<模型 id>/manifest.json`（也附在 main 分支）。网页先从 jsDelivr 下载，失败时改从网站自己的域名下载。
各模型的出处与许可见对应目录的 README.txt。

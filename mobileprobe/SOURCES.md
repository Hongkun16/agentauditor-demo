# 素材来源与证据说明

## 论文参考图

以下四张图片按原项目记录，来自 NDSS’27 MobileProbe 研究素材。中文版未编辑这些图片；下表保留原项目的来源路径及 SHA-256 记录。原始文件名与校验值保留；本文档中的参考图不属于手机回放帧。

| Demo asset | Original file | SHA-256 |
| --- | --- | --- |
| `assets/malicious1.png` | `Malicious1.png` | `dcbb39e730d2ad85d772be3d585a50fa6f1cd5fa8b37dc00534edfe4b37f3b88` |
| `assets/malicious2.png` | `Malicious2.png` | `f600e6ababb65dd0434def49afe91f9909766bd9db8d77d4f449d33bfe3877fb` |
| `assets/fake_dialog1.png` | `fake_dialog1.png` | `c6956a896e64515667eed1946dbb869d4141adeafbf7d2a937ec6ce092b43e75` |
| `assets/fake_dialog2.png` | `fake_dialog2.png` | `cfc855fbc485c7c2645f574b7299b2c0da2a1793ae94d7017e66100c66d78eff` |

## 手机回放截图

`assets/replays/<case>/` 中的图片为单独手动采集的手机截图，不是论文参考图。中文版本未修改截图像素，只调整网页显示、中文字幕、操作提示及回放节奏。

画面中的点击与滑动提示由网页单独绘制，部分坐标为推断目标位置。这些提示用于演示动作，不应解释为真实 AI 执行日志。

## 案例含义

恶意文本案例的入口是邮件正文、卖家商品描述。假弹窗案例假设用户运行了被篡改的第三方应用，弹窗位于该应用内部，不是覆盖任意应用的 Android 系统弹窗。

邮件案例显示额外短信；购物案例显示数量变为两份，未提交或支付。两个假弹窗案例只显示接受攻击者提示并关闭弹窗，不推断后续关键词保存或信息发送结果。

## 离线数据

`app.js` 中内嵌中文清单，以支持直接双击 HTML。内嵌清单与 `assets/replays/` 中的 JSON 一致。关键攻击画面在 1× 倍速下至少停留 10 秒。

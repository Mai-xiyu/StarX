# StarX

学习通 LSPosed 模块公开仓库。

这个仓库主要用于发布公开版本、收集用户 issue 与公测反馈。

## 反馈入口

- 最新公开版本：<https://github.com/Mai-xiyu/StarX/releases>
- 提交问题或建议：<https://github.com/Mai-xiyu/StarX/issues/new/choose>
- 公测反馈清单：<https://github.com/Mai-xiyu/StarX/blob/main/PUBLIC_TEST_CHECKLIST.md>

## 提 issue 前建议准备的信息

- StarX 版本
- 学习通版本
- Android 版本、机型、LSPosed 版本
- 具体页面入口和复现步骤
- 复现后的日志、截图或录屏

建议在复现后导出日志：

```powershell
adb logcat -d -s StarX:D *:S
```

如果问题与签到、题库或考试页面相关，尽量同时说明：

- 页面类型，例如 H5 二维码签到、原生二维码签到、拍照签到、作业页、考试页
- 题库协议类型，例如 LemTk、tikuAdapter、ZXSeek / Wkexam
- 是否稳定复现，以及大概复现概率

## 公测重点

当前更建议优先反馈这些回归风险较高的项目：

- 动态题库源新增、删除、保存后回读
- tikuAdapter 根地址与协议类型切换
- ZXSeek 预置源与 token 填写
- H5 二维码签到与原生二维码签到分流
- 拍照签到自动上传
- 定位签到自动抓取与手动定位
- 考试搜题、选项识别与题型识别

详细清单见 <https://github.com/Mai-xiyu/StarX/blob/main/PUBLIC_TEST_CHECKLIST.md>。


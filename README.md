# Creative Prompt Director

一个中文优先、默认离线的 AI 视觉提示词 Skill，面向：

- AI 短剧、广告片、分镜和图生视频提示词
- 产品白底图、Hero 图、生活方式图、细节图和组图
- 连续性、产品保真、版权/IP、隐私和宣传 claims 审核

## 安全边界

本仓库只包含 Markdown 和 UI 元数据：

- 不调用图片或视频 API
- 不读取或保存 API Key
- 不自动上传剧本、产品图、人物参考图或品牌素材
- 不安装第三方依赖，不执行 Shell/Python 生成器

生成图片或视频时，请由用户明确选择服务，并在服务自身的官方界面或经过审计的集成中完成提交。

## 使用

将本仓库中的 Skill 目录安装到支持 Skills 的 AI 客户端，然后使用：

```text
使用 $creative-prompt-director，把这个故事改成60秒竖屏短剧分镜。
```

或：

```text
使用 $creative-prompt-director，为这款产品设计白底主图和三张生活方式图。
```

不同客户端的 Skills 目录位置不同；安装前应先查看客户端自己的 Skill 安装说明。

## 许可证

MIT License，见 [LICENSE](LICENSE)。方法论来源和安全排除项见 [references/prior-art.md](references/prior-art.md)。

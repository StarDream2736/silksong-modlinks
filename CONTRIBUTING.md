# 贡献指南

感谢你对Silksong ModLinks的贡献！

## 提交Mod

### 1. 准备工作

- Fork此仓库
- 确保你的Mod已在GitHub上发布Release
- 计算所有平台文件的SHA256哈希值

### 2. 计算SHA256

**Windows PowerShell:**
```powershell
Get-FileHash .\YourMod.zip -Algorithm SHA256 | Select-Object -ExpandProperty Hash
```

**Linux/Mac:**
```bash
shasum -a 256 YourMod.zip
```

### 3. 编辑ModLinks.xml

在 `<ModLinks>` 标签内添加你的Mod条目：

```xml
<Manifest>
  <Name>YourModName</Name>
  <Description>你的Mod描述</Description>
  <Version>1.0.0</Version>
  <Authors>
    <Author>YourName</Author>
  </Authors>
  <Links>
    <Windows SHA256="计算出的哈希">https://github.com/you/mod/releases/download/v1.0.0/YourMod.zip</Windows>
  </Links>
  <Dependencies>
    <!-- 如果有依赖 -->
  </Dependencies>
  <Repository>https://github.com/you/mod</Repository>
  <Tags>
    <Tag>Gameplay</Tag>
  </Tags>
</Manifest>
```

### 4. 提交Pull Request

- 创建新分支: `git checkout -b add-your-mod-name`
- 提交更改: `git commit -m "Add YourModName v1.0.0"`
- 推送分支: `git push origin add-your-mod-name`
- 在GitHub上创建Pull Request

### 5. 等待审核

维护者会验证：
- XML格式正确性
- SHA256哈希准确性
- 下载链接可用性
- Mod安全性

## 行为准则

- 尊重社区成员
- 不提交恶意代码
- 确保Mod描述准确
- 及时响应审核意见

## 问题反馈

如有疑问，请创建Issue或在Pull Request中评论。

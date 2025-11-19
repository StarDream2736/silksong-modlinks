# Silksong ModLinks

这是 [Chrysalis](https://github.com/StarDream2736/Chrysalis) Mod管理器的官方Mod索引仓库。

## 📝 文件说明

- **ModLinks.xml**: Mod索引文件，包含所有可用Mod的信息
- **ApiLinks.xml**: BepInEx索引文件，包含BepInEx下载链接和配置


## 📋 XML格式规范

### ModLinks.xml 基本结构

```xml
<Manifest>
  <Name>ModName</Name>
  <Description>Mod描述</Description>
  <Version>1.0.0</Version>
  <Authors>
    <Author>作者名</Author>
  </Authors>
  <Links>
    <Windows SHA256="哈希值">下载链接</Windows>
  </Links>
  <Repository>仓库地址</Repository>
  <Dependencies>
    <Dependency>依赖的Mod</Dependency>
  </Dependencies>
  <Tags>
    <Tag>标签</Tag>
  </Tags>
</Manifest>
```

## 📞 联系方式

- 问题反馈: [创建Issue](https://github.com/StarDream2736/silksong-modlinks/issues)
- Mod提交: 通过Pull Request提交

## 📄 许可证

本仓库采用 GPL-3.0 许可证。

---

*Made for Hollow Knight: Silksong modding community*

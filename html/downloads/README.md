# 下载文件夹说明

## 如何上传exe文件

1. **将您的exe文件复制到此文件夹** (`my-web/downloads/`)

2. **编辑 `download.html` 文件**，在JavaScript的 `downloadFiles` 数组中添加文件信息：

```javascript
const downloadFiles = [
    {
        name: "您的应用程序名称",
        description: "应用程序的详细描述",
        version: "1.0.0",
        filename: "your-app.exe",  // 您的exe文件名
        size: "10.5 MB"  // 文件大小（可选）
    }
];
```

3. **保存文件后**，访问网站的 `/download.html` 页面即可看到下载按钮

## 注意事项

- 确保exe文件名与配置中的 `filename` 字段完全一致
- 文件大小信息是可选的，但建议填写以便用户了解
- 可以添加多个下载项，只需在数组中添加更多对象即可

# Introduction

### 全局安装
```
npm install gitbook-cli -g
```

### 初始化
```
gitbook init
```

### 修改端口号并启动
```
gitbook serve --port 8000
```

### book.json配置
```json
{
  "title": "我的第一本电子书哈哈",
  "description": "用 GitBook 制作的第一本电子书！",
  "isbn": "978-3-16-148410-0",
  "language": "zh",
  "direction": "ltr",
  "pluginsConfig": {
    "theme-default": {
      "showLevel": true
    }
  }
}
```

### 使用
给目录添加数字
```json
{
  "pluginsConfig": {
    "theme-default": {
      "showLevel": true
    }
  }
}
```

### 打包
```
gitbook build
```

### 用gh-pages发布到github分支预览项目
```bash
# 先全局安装
npm install gh-pages -g

# 安装到项目里
npm install gh-pages --save-dev

# 把打包后文件夹 _book 发布到 gh-pages 分支
gh-pages -d _book
```

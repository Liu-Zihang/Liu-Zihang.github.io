# 发布到 GitHub Pages（个人主页 xxx.github.io）

## 1. 在 GitHub 上建仓库

1. 打开 https://github.com/new
2. **Repository name** 填：`你的用户名.github.io`（例如你的 GitHub 用户名是 `Liu-Zihang`，就填 **Liu-Zihang.github.io**）
3. 选 **Public**，不要勾选 “Add a README file”
4. 点 **Create repository**

## 2. 本地添加远程并推送

在终端里进入项目目录，执行（把 `Liu-Zihang` 换成你的 GitHub 用户名）：

```bash
cd /Users/lzh/Desktop/html

# 添加远程仓库（替换成你的用户名）
git remote add origin https://github.com/Liu-Zihang/Liu-Zihang.github.io.git

# 推送到 GitHub
git push -u origin main
```

如果提示认证，按提示用浏览器或 Personal Access Token 登录即可。

## 3. 开启 GitHub Pages

1. 打开你的仓库页面，点 **Settings** → 左侧 **Pages**
2. 在 **Source** 里选 **Deploy from a branch**
3. **Branch** 选 `main`，文件夹选 **/ (root)**，点 **Save**
4. 等一两分钟，访问 **https://你的用户名.github.io** 即可看到你的个人主页

---

之后改完页面，提交并推送即可更新网站：

```bash
git add .
git commit -m "更新内容"
git push
```

# 高考备考材料库

按 **科目 → 专题** 组织的高中复习讲解材料库，面向高中学生免费开放，通过 GitHub Pages 发布。

## 内容组织

```
gaokao/
├── index.html              # 落地页（GitHub Pages 首页，按科目列出材料）
├── README.md               # 本说明
├── .nojekyll               # 关闭 Jekyll，保证文件原样托管
└── 物理/
    ├── 3.1 运动学复习讲解-课件.html
    └── images/             # 课件引用的图片
```

- 每个科目一个顶层目录（物理 / 数学 / 化学 …）
- 每个专题一个课件（或若干相关文件），同级 `images/` 放该课件用到的图片
- 课件为单文件 HTML，公式走 MathJax CDN，可直接在浏览器打开

## 在线访问

发布会自动生成 GitHub Pages 地址（仓库 Settings → Pages，来源 `main` 分支根目录）：

> https://na57.github.io/gaokao/

## 本地预览

直接双击 `index.html` 即可；或在本目录起一个静态服务：

```bash
python3 -m http.server 8000
# 浏览器打开 http://localhost:8000
```

## 提交规范

- 新增科目：新建 `科目名/` 目录
- 新增专题：在对应科目目录下放入课件 HTML，并把用到的图片放进同级的 `images/`
- 同步更新 `index.html`，把新材料加进对应科目列表

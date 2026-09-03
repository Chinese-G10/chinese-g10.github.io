# 十年级中文复习站

Lynn 的十年级中文课复习材料，托管在 GitHub Pages。
**这个站只放十年级的东西**，九年级在另一个站，两边互不相通。

网址：https://chinese-g10.github.io/

## 怎么建这个站（只做一次）

1. GitHub 右上角 **+ → New organization → 选免费方案**
   - Organization name：`Chinese-G10`
   - This organization belongs to：**My personal account**
2. 在这个 Org 里 **New repository**，仓库名必须**正好等于** `chinese-g10.github.io`
   （全小写、带 `.github.io` 后缀，错一个字符 Pages 就不生效），可见性选 **Public**
3. 仓库页 → **Add file → Upload files**，把本文件夹里的东西全拖进去 → Commit
4. Settings → Pages，确认 Source 是 `Deploy from a branch` / `main` / `/ (root)`
5. 等 1–2 分钟，网址就通了

## 为什么是 Org 而不是新 repo

同一个账号下开新 repo，网址会是 `lynn-ccmimi.github.io/仓库名/`，
学生把地址栏后面删掉还是能看到九年级的站。
用 Org 就有了自己的域名 `chinese-g10.github.io`，删到根也只有十年级。

> ⚠️ 这仍然是「分开域名」，不是「加权限」。GitHub Pages 是公开托管，
> 网址被转发出去谁都能打开。复习资料不涉密，这样够用。
> 私有仓库也不行——Pages 从私有仓库发布的站点本身仍然是公开的，而且要付费套餐。

## 什么不能上传

**课堂用的 PPT（`*_课堂.html`）一律不上传。**
那里面有考试原题原句，放到学生能打开的网址上等于漏题。只上传给学生的复习手册。

## 结构

```
index.html            首页（唯一需要手改的文件）
g10-mt1/index.html    第一阶段 MT 复习手册
```

**文件夹命名规则**：全小写，只用英文和连字符，例：`g10-mt1`、`g10-l3`、`g10-oral`。
中文文件名在网址里会变成 `%E5%8F%A3...` 一长串，学生没法打。

## 加一课新的怎么做

1. 新的复习 HTML 复制进来，放成 `课次名/index.html`，例：`g10-l3/index.html`
2. 打开 `index.html`，复制一整块 `<a class="card">…</a>`，改四个地方：
   - `href` — 文件夹名，**末尾带斜杠**，例 `"g10-l3/"`
   - 两个 `<span class="tag">` — 年级、课次
   - `h2` / `sub` / `what` 三行文字
3. Add file → Upload files 拖上去（同名自动覆盖，不用先删）
4. 等 1–2 分钟生效

## 注意

- 复习 HTML 是自包含的，不依赖任何外部文件，单文件 70 KB 左右
- 手机和 iPad 都适配过：窄屏时左侧目录收成抽屉，底部有 ☰ Contents 按钮

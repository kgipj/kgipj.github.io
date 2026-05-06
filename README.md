# Navi's Notes

Hugo + Archie 版本的個人部落格。

## 本機預覽

```sh
hugo server -D
```

## 建立新文章

```sh
hugo new posts/my-new-post.md
```

文章會出現在 `content/posts/`，用 Markdown 編輯。

## 發布到 GitHub Pages

把這個資料夾裡的內容上傳到 GitHub repo 最外層，然後到 repo 的：

`Settings` -> `Pages` -> `Build and deployment`

把 Source 改成 `Deploy from a branch`，Branch 選：

```text
gh-pages / (root)
```

之後每次推到 `main`，GitHub Actions 會自動 build Hugo，並把網站發布到 `gh-pages` 分支。

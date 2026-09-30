![工作坊完成徽章](https://img.shields.io/badge/GitHub_Copilot_實戰工作坊-已完成-1F883D?style=for-the-badge&logo=githubcopilot&logoColor=white)

# 待辦清單 Web App

這是在 GitHub Copilot 實戰工作坊完成的待辦清單 Web App。專案以精簡的前端技術實作日常待辦管理，並透過主題切換、篩選與瀏覽器本機儲存，練習從需求描述到功能驗證的完整開發流程。

## 線上展示

GitHub Pages：`https://<你的帳號>.github.io/<你的repo名稱>/`

## 功能

- 新增待辦事項，並阻止空白內容送出。
- 勾選或取消勾選完成狀態；已完成項目會顯示刪除線並淡化。
- 刪除單筆待辦事項。
- 顯示未完成項目數量，計數不受目前篩選條件影響。
- 依「全部」、「未完成」或「已完成」篩選清單，並在清單或篩選結果為空時顯示提示。
- 切換淺色與深色模式；尚未手動選擇時跟隨作業系統偏好，手動選擇會記住偏好。
- 將待辦資料與手動主題偏好保存至 `localStorage`，重新整理後仍可保留。
- 採用置中卡片版面並支援手機螢幕。

## 技術

- 使用 HTML、CSS 與原生 JavaScript 建置，沒有使用前端框架或套件。
- CSS 以 `:root` 變數管理色彩，並支援淺色與深色主題。
- 待辦資料與主題偏好使用瀏覽器 `localStorage` 保存。
- 不依賴外部 CDN 或建置流程；應用程式可離線開啟。

## 開發方式

- 使用 GitHub Copilot Agent Mode 根據功能需求建立並迭代待辦清單介面與互動。
- 透過 `.vscode/mcp.json` 設定 Microsoft Learn 與 GitHub MCP Server，作為查閱文件與 GitHub 專案資訊的工具連線設定。
- 以 `.github/copilot-instructions.md` 記錄專案技術限制、程式風格與協作規則。
- 以 `.github/prompts/fix-issue.prompt.md` 定義可重複使用的 issue 修復流程，包含讀取 issue、提出計畫並等待確認、建立分支、實作、驗證、提交推送及建立 Pull Request。
- 透過瀏覽器操作驗證主要互動，並使用 Git 分支、提交與 Pull Request 管理變更。

## 我學到什麼

- 先把需求與成功條件寫清楚，有助於讓 Agent Mode 產出更貼近預期的修改。
- MCP 設定能讓工具連線到文件與 GitHub 等外部資訊來源。
- 將專案規則與重複流程寫成 Markdown，能讓後續協作更一致、流程更容易重用。
- 透過瀏覽器實際操作驗證，比只確認程式碼能執行更能發現使用流程中的問題。
- 使用分支、提交與 Pull Request，可以清楚追蹤並檢視每次功能變更。
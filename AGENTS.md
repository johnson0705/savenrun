# AGENTS.md

本 repo 尚未建立完整 Claude/Codex 規則。Codex 進入後以保守工程流程為準。

## 啟動順序

1. 執行 `git status --short` 與 `git branch --show-current`。
2. 掃描專案結構：`README.md`、package/build 設定、測試目錄、部署腳本。
3. 先讀現有程式碼與測試，再提出修改方案。
4. 沒有明確需求時，不新增大型框架、不重排目錄、不改 release/deploy 流程。

## 開發規則

- 優先延續現有技術棧與命名風格。
- 不寫死 secrets、帳號、絕對路徑或環境專屬設定。
- 修改使用者可見行為時，同步檢查 README/docs 是否需要更新。
- 不碰 unrelated dirty files。

## Commit

- 未經使用者明確要求，不自動 commit、tag、push。
- 若要 commit，只 stage 本次任務相關檔案。
- 交付時回報改動、驗證、未驗證項與風險。

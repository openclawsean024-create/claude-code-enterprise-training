# Changelog · claude-code-enterprise-training PRD

所有 PRD / SPEC 變更記錄於此。最新在上。

---

## [v3.0.2] · 2026-09-07 · fleet-upgrade

### Added（新增）
- §A 部署契約（Fleet 規格，8 個子節）
  - §A.1 部署目標表（Pages + Vercel 雙軌）
  - §A.2 2 個靜態入口檔案清單
  - §A.3 連結檢查結果表（0 失效）
  - §A.4 GHA Workflow 觸發說明
  - §A.5 環境變數表（無）
  - §A.6 部署後驗證 checklist
  - §A.7 雙軌說明（Pages 靜態 + Vercel 既有產線）
  - §A.8 URL 對照（Pages + Vercel + GitHub）
- 版本號升級 v2.2.2 → v3.0.2
- 標頭加入 fleet-upgrade 標記 + 部署目標明確為 GitHub Pages

### Changed（變更）
- 升級對齊 SPEC v3.0 契約（fleet 統一規格）
- 部署目標從 Vercel 單軌 → **Pages（靜態）+ Vercel（既有產線）雙軌**
- GHA workflow 新增 Pages 自動部署（4 jobs: lint / test / build / deploy）

### Status
- 2 個 HTML 入口：✅ all served
- 內部連結：✅ 0 失效
- 雙軌部署：✅ Pages（靜態）+ Vercel（既有產線）並存
- GHA: ✅ ci.yml 建立（4 jobs, 靜態 Pages deploy）

---

## [v2.2.2] · 2026-07-19 · sweet-spot-driven rewrite by Sophia CPO

### Added
- §0 改版摘要（sweet spot 5 問體檢，3/10，建議 kill）
- §1.1 問題陳述：「中小企業導入 Claude Code 後 ROI 為零」這個被忽略的痛點
- §1.3 核心價值主張：「7 天帶企業導入 Claude Code 的陪跑教練，非錄製課程平台」
- §1.5 Non-Goals：不做通用 AI 課程、不做證照、不做個人訂閱（聚焦 B2B 陪跑）
- §3.1 MVP：從 50 堂課程縮減為 1 個垂直產業（餐飲 POS 中小企業）+ 7 天工作坊
- §7.2 ADR-005：為何不做錄製課程平台
- §11 市場驗證：5 場餐飲/零售業主訪談 + 1 個 Landing Page + 1 個 PTT/Threads 貼文
- §15 完整 sweet spot 體檢報告與對沖策略
- §15.3 對沖策略 + §15.4 退出策略 + §15.5 Open Questions + §15.6 ROI 估算（18 個月 ROI = 880%）

### Status
- 純靜態 HTML 2 個入口（index.html + dashboard.html）
- 部署目標：Vercel（既有產線，410K+ 觀看流量對接）
- 對接市場：410K+ 觀看（柚智夫妻 X 雷蒙三十合作）

### Notes
- sweet spot：3/10｜建議動作：戰略收斂（不做通用 AI 課程，聚焦 B2B 陪跑）

---

## [v1.0] · 2026-05 · init

- 中文 Claude Code 企業內訓 50 堂通用課程
- 對接 410K+ 觀看市場驗證模式
- Vercel 部署（CLI ZIP）

# 六小時、50°C：法國超市冷鏈被遠端加熱，缺口在哪裡

導讀 2026-10-11／12 法國 Intermarché、Système U、Leclerc 等超市冷藏設備遭網路攻擊事件：數字為何對不上、官方（CERT-FR、巴黎檢察署）與廠商（Danfoss）各說了什麼、哪些仍無答案，以及冷鏈管理者的自查清單。資訊截至 2026-10-13。

## 200字介紹

2026 年 10 月 11 日夜間到 12 日，法國多家連鎖超市的冷藏櫃被遠端調到約 50°C，受災門市必須清空、請執達員驗證後銷毀食品。本文把各方說法並排：受災門市數從約一百到三百不等，多半是統計口徑不同；法國 CERT-FR 確認多起 Danfoss AK-SM 與 AK-SC 設備遭入侵，Danfoss 說受害的是停止更新的舊品，或沒有更新韌體的現行機型；入侵手法、攻擊者、動機與火災規模都還沒有公開答案。文末附上依 CERT-FR 與 CISA 建議整理的冷鏈自查清單：檢查對外暴露、斷開直接連線、盤點停更設備、獨立偵測、事前演練與採購合約條款。

## 檔案

| 檔案 | 說明 |
|---|---|
| `index.html` | 導讀網頁（CSS 內嵌；Mermaid 由 CDN 載入，失效時顯示圖表原文） |
| `france_fridge_cyberattack_danfoss.md` | 導讀 Markdown 原稿 |
| `images/summary-16x9.png`、`images/summary-mobile.png` | 一圖看懂（桌面 16:9、手機 9:16） |
| `images/risk-conditions-*.png`、`images/dos-contrast-*.png` | 風險段落配圖（各有桌面 16:9、手機 9:16） |

## 原始資料

- Lycos 彙整頁（33 則報導）：https://news.lycos.fr/sujet/cyberattaque-des-frigos-d-intermarche-u-et-leclerc-vises-98684
- Anadolu Ajansı：https://www.aa.com.tr/fr/france/france-une-cyberattaque-d-ampleur-perturbe-les-syst%C3%A8mes-frigorifiques-de-plusieurs-enseignes-de-grande-distribution/4086077
- 逐字稿：不適用（文章型來源）。

## 重要來源

- CERT-FR 警報 CERTFR-2026-ALE-012（官方）
- CISA ICSA-25-140-03、Danfoss DSA-2025-03-01（官方漏洞公告）
- Cooling Post（Danfoss 聲明）、AFP、Reuters（經 CBS／ABC 轉述）、Le Monde、franceinfo
- Claroty Team82 研究

完整清單見導讀文末。

## 網址

https://lushinshang.github.io/france_fridge_cyberattack_danfoss/

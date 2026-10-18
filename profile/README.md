# TradingNote

台股市場儀表板與投資筆記工具：https://www.tradingnote.tw

## 產品

- 台股盤後與總經評分：每個交易日 15:30 更新三大法人、外資期貨、選擇權 PCR、台灣 VIX 等指標，並彙整成一個總經評分。
- 台股 AI 日報：每天由 Gemini 依當日盤後資料產生大盤結論、外資動向與風險情境；另有總經新聞解讀，以及「巴逆逆觀察」（AI 整理社群反指標人物的 Facebook 操作，反向作為參考訊號）。
- K 線圖與版面：技術指標、畫線標註、多股比較，版面可儲存；新聞可連結到個股，看圖時對照當天事件。
- 筆記、投資報告與交易紀錄：筆記可附圖片與 PDF，報告可分享或匯出 PDF，交易旅程與交易日記記錄每筆交易的進出與復盤。
- 其他：市場總覽、供應鏈流向圖、觀察清單、股票農民曆與財經行事曆。

## Repositories

除了 `.github` 之外都是 private repo，點進去會是 404。

| Repo | 說明 | 技術 |
| --- | --- | --- |
| `trading-frontend` | 主站 www.tradingnote.tw | Next.js 15、React 19、TypeScript、Tailwind CSS 4、klinecharts |
| `trading-backend` | 主後端 API（gurula.cc）：會員、新聞、筆記、報告、版面、交易紀錄 | Java、Spring Boot |
| `trading-tw-market` | 台股盤後資料 API（api.tradingnote.tw）與獨立前端（stock.tradingnote.tw）：抓取 TWSE／TAIFEX／MOPS 資料、總經評分、AI 解盤 | Python、Flask、PostgreSQL、React、Vite |
| `trading-source` | 監看 YouTube 財經頻道等來源，用 Gemini 產生摘要與總經晨報，推送到後端 | Python、FastAPI |
| `Tideline` | 情境分析引擎：從新聞與分析師觀點偵測分歧、推演多條情境、產生社群圖卡（開發中） | Python、Node.js |
| `trading-device` | ESP32-S3 股票顯示裝置韌體，32×16 LED 點陣面板 | C++、PlatformIO |
| `trading-ai` | 多代理人個股研究實驗（LangGraph，已封存） | Python |

## 團隊

- [Aaron](https://github.com/eepson123tw) — 前端
- [YF](https://github.com/YFCKevin) — 後端

2025 Q2 開始開發，2025 Q4 上線。

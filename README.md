# n8n Workflows

## 日幣匯率每日通知
每天早上 9 點自動抓取日圓兌台幣匯率，由 Gemini 產生通知訊息後推播到 Discord。

流程：Schedule Trigger → HTTP Request（匯率 API）→ Edit Fields → Basic LLM Chain（Gemini）→ Discord

技術：n8n（Docker 自架）、REST API、Google Gemini、Discord Webhook
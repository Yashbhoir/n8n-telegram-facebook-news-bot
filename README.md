# n8n News Automation Bot

This workflow automates the process of posting news articles from an RSS feed to Facebook with Telegram approval.

## Features
- Fetches news from RSS feed
- Sends news URL and date to Telegram for approval
- Allows user to approve/reject news via Telegram
- Posts approved news to Facebook with image and caption
- Fully automated with n8n workflow

## Workflow File
The workflow JSON file: `facebook_publish.json`

## 🚀 How to Import This Workflow into n8n

1. Open your n8n instance (cloud or self-hosted).
2. Go to **Workflows** → **Import from File**.
3. Upload the provided file: `rss-news-workflow.json`.
4. Once imported, configure the following credentials:
   - **Telegram Bot Token** (create via [BotFather](https://core.telegram.org/bots#6-botfather))
   - **Facebook Graph API Token** (create in [Meta for Developers](https://developers.facebook.com/))
5. Adjust the **RSS Feed URL** and scheduling interval if needed.
6. **Activate Workflow** → n8n will now:
   - Fetch latest news from the RSS feed.
   - Send each item to Telegram for approval/rejection.
   - Post approved items to Facebook with image and caption.


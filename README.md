# n8n News Automation Bot

This workflow automates the process of posting news articles from an RSS feed to Facebook with Telegram approval.

## Features
- Fetches news from RSS feed
- Sends news URL and date to Telegram for approval
- Allows the user to approve/reject news via Telegram
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
  

### Telegram Approval Flow
Example notification with approve/reject option:

Steps:

1.	Check the latest notification from Animebot chat, it's about "ansatsusha de aru ore no status ga" anime
2.	Click on the link provided by the bot to check out news from the RSS feed source directly
3.	The provided image is the source of the news 
4.	Go back to the bot and approve the news article, click open 
5.	Acknowledgment for the approved news by the n8n webhook is provided 
6.	The next news article to approve or reject has appeared on chat


<img width="607" height="1350" alt="image" src="https://github.com/user-attachments/assets/68157bd8-f331-4f27-8952-af83916300fa" />

<img width="607" height="1350" alt="image" src="https://github.com/user-attachments/assets/e54e741d-7f61-4bc5-b32a-4cfae08139f1" />

<img width="608" height="1350" alt="image" src="https://github.com/user-attachments/assets/b338dc1c-5cd7-4df9-a161-42f3b7679735" />

<img width="608" height="1350" alt="image" src="https://github.com/user-attachments/assets/7244928c-666b-40cf-8f3b-feb3999f8d4a" />

<img width="608" height="1350" alt="image" src="https://github.com/user-attachments/assets/5f1f8bb6-d442-451d-8309-e843facf9e84" />

<img width="607" height="1350" alt="image" src="https://github.com/user-attachments/assets/c37d51e3-bd6f-422a-bb79-7ca1af4567d9" />


### Facebook Post
Example of approved news published to Facebook:

## This is my page on Facebook

<img width="607" height="1350" alt="image" src="https://github.com/user-attachments/assets/3900e054-86d6-4748-aaa3-d2c579586279" />

## The approved news article has been successfully published on page

<img width="607" height="1350" alt="image" src="https://github.com/user-attachments/assets/f0673909-81e8-462c-ae4c-1909ef9578ba" />










# shivam

## How to Check Your Token Usage Percentage

Depending on which service you are using, here is where you can check how many tokens you have consumed and what percentage of your quota remains:

---

### GitHub Copilot

GitHub Copilot is a seat-based subscription and does **not** expose a per-user token counter.  
To manage your Copilot seats and billing:

1. Go to **GitHub** → your profile picture → **Settings**.
2. Click **Billing and plans** (for personal accounts) **or** navigate to your **Organization** → **Settings** → **Billing**.
3. Under the *GitHub Copilot* section you can see active seats, usage, and cost.

GitHub Copilot Business/Enterprise admins can also review seat usage at:  
`https://github.com/organizations/<org>/settings/copilot/seat_management`

---

### OpenAI API (GPT models)

1. Log in at <https://platform.openai.com>.
2. Click your account icon in the top-right corner → **Usage**.
3. The **Usage** dashboard shows:
   - Total tokens used (prompt + completion) per day/month.
   - Cost breakdown by model.
4. To see your remaining free-tier credits or hard-limit, go to **Settings** → **Billing** → **Usage limits**.

You can also query usage programmatically via the OpenAI API:
```
GET https://api.openai.com/v1/usage?date=YYYY-MM-DD
Authorization: Bearer <your-api-key>
```

---

### Anthropic Claude API

1. Log in at <https://console.anthropic.com>.
2. Navigate to **Usage** in the left sidebar.
3. The dashboard shows token consumption broken down by model and date.

---

### Google Gemini / Vertex AI

1. Open the [Google Cloud Console](https://console.cloud.google.com).
2. Go to **APIs & Services** → **Quotas & System Limits**.
3. Search for the relevant API (e.g., *Generative Language API* or *Vertex AI*).
4. Current usage vs. quota limit is shown as a percentage.

---

### General Tips

- Set **spending limits / hard caps** in each provider's billing settings to avoid unexpected charges.
- Use **alerts** (available in OpenAI, GCP, and Azure) to get notified when you reach a certain percentage of your quota.
- For local models (e.g., Ollama, LM Studio) there is no token quota — you are limited only by your hardware.

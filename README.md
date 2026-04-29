# 🤖 Chirag AI — Business Coach Agent

A fully functional AI chat agent for Coach Chirag Chhabra, built on Claude AI.

---

## 📁 Project Structure

```
chirag-agent/
├── api/
│   └── chat.js          ← Secure backend (calls Claude API)
├── public/
│   ├── index.html       ← Beautiful chat UI
│   └── embed.html       ← Widget embed code generator
├── vercel.json          ← Vercel deployment config
└── README.md
```

---

## 🚀 Deploy to Vercel (Step-by-Step)

### Step 1 — Get your Claude API Key
1. Go to https://platform.claude.com
2. Sign up (free $5 credits included)
3. Go to **API Keys** → Click **Create Key**
4. Copy the key (starts with `sk-ant-...`)

### Step 2 — Deploy to Vercel
1. Go to https://vercel.com and sign up (free)
2. Click **"Add New Project"**
3. Upload this folder (drag & drop or connect GitHub)
4. Before deploying, go to **Environment Variables**
5. Add this variable:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** `sk-ant-YOUR_KEY_HERE`
6. Click **Deploy** ✅

### Step 3 — Get your live URL
After deployment, Vercel gives you a URL like:
`https://chirag-agent-xyz.vercel.app`

Your agent is now LIVE! 🎉

---

## 🌐 Add to Chirag's Website

1. Visit `https://your-vercel-url.vercel.app/embed.html`
2. Copy the embed code shown
3. Replace `YOUR-VERCEL-APP` with your actual Vercel URL
4. Paste into Chirag's WordPress site before `</body>` tag
5. A 🤖 chat bubble will appear on every page!

---

## 💰 Expected Cost

Using Claude Haiku 4.5 (the cheapest model):
- ~500 conversations/month = **under ₹300–500/month**
- First month likely free (within $5 free credits)

---

## 🔧 Customization

To change the AI's personality or knowledge, edit the `SYSTEM_PROMPT` in `api/chat.js`.

To change colors/branding, edit the CSS variables at the top of `public/index.html`:
```css
--gold: #C9973A;
--dark: #0D0B08;
```

---

Built with ❤️ using Claude AI (Haiku 4.5) + Vercel Serverless Functions

# 🤖 Ask Chiderah — AI CV Chatbot

> An AI-powered chatbot that lets recruiters and clients chat with a digital version of me — instead of reading a static CV.

**Live demo:** [chiderah.github.io/ask-chiderah](https://chiderah.github.io/ask-chiderah) *(update after deployment)*

---

## What This Is

Most CVs get skimmed in 6 seconds. This project flips that dynamic — recruiters can have an actual conversation with an AI trained on my experience, skills, and professional background.

Built to demonstrate:
- **Prompt engineering** — crafting a system prompt that accurately represents a real professional identity
- **Claude API integration** — direct browser-to-API calls with conversation history
- **Frontend development** — clean, dark-mode UI with no frameworks or build tools
- **AI product thinking** — designing an experience around a real-world use case

---

## Features

- 💬 Real-time AI chat powered by Claude (claude-sonnet)
- 🧠 System prompt trained on my actual CV, skills, and achievements
- 📜 Conversation history maintained across turns
- 💡 Suggested questions to guide recruiters
- 🔑 API key stored locally in the browser (never transmitted elsewhere)
- 📱 Fully responsive — works on mobile and desktop
- ⚡ Zero dependencies, zero build step — single HTML file

---

## Tech Stack

| Layer | Technology |
|---|---|
| AI Model | Claude claude-sonnet (Anthropic API) |
| Frontend | Vanilla HTML, CSS, JavaScript |
| Fonts | Syne + DM Mono (Google Fonts) |
| Hosting | GitHub Pages |
| State | In-browser (localStorage for API key, JS array for chat history) |

---

## Running Locally

No build tools needed. Just clone and open:

```bash
git clone https://github.com/chiderah/ask-chiderah.git
cd ask-chiderah
open index.html
```

You'll be prompted to enter your Anthropic API key on first load. Get one free at [console.anthropic.com](https://console.anthropic.com).

---

## Deploying to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your chatbot will be live at `https://yourusername.github.io/ask-chiderah`

---

## How It Works

```
User types a question
       ↓
Browser sends message + conversation history to Anthropic API
       ↓
System prompt provides Chiderah's professional context to Claude
       ↓
Claude responds in first person as Chiderah
       ↓
Response rendered in chat UI, added to conversation history
```

The key file is the **system prompt** inside `index.html` — it contains my full professional profile, key achievements (including the CBN T+1 Cheque Clearing Reform), skills, and communication style guidelines. This is the core prompt engineering work.

---

## Customising for Your Own CV

Want to fork this and make your own AI CV chatbot?

1. Fork this repo
2. Open `index.html`
3. Find the `SYSTEM_PROMPT` constant and replace the content with your own professional details
4. Update the header name and badges in the HTML
5. Deploy to GitHub Pages

The system prompt structure I used:
- Personal intro + current role
- Key achievements (with specifics and impact)
- Skills and tools (categorised)
- Notable projects
- Communication style guidelines
- What you're open to (for recruiters)

---

## About Chiderah

**Chiderah Onwudinjo** is a Lagos-based Digital Marketing & AI Content Specialist with experience spanning institutional finance (Central Bank of Nigeria), digital marketing, and AI automation.

- 🏢 Currently: Digital Marketing & AI Content Specialist at Leind Studio
- 🔥 Founder: [theFIREbrand](https://thefirebrand.agency) — AI-powered digital marketing agency
- 🏦 Previously: Clearing, Treasury & Customer Care Officer at the CBN
- 📍 Lagos, Nigeria | Open to remote roles globally

**Connect:**
- LinkedIn: [linkedin.com/in/chiderah](https://linkedin.com/in/chiderah) *(update link)*
- Email: *(add your email)*

---

## License

MIT — feel free to fork, adapt, and build your own version.

---

*Built with Claude API · Deployed on GitHub Pages*

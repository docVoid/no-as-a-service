# no-as-a-service

❌ No-as-a-Service (NaaS)

Welcome to **No-as-a-Service** – the graceful, sarcastic, Shakespearean, and multilingual way to say "no".

Because sometimes, just "No" isn't enough.

---

## 🧐 What is this?

**No-as-a-Service (NaaS)** is a lightweight C# API that serves various humorous, polite, blunt, or dramatic versions of the word "no". Designed for developers who want to decline things *elegantly* in their apps, tools, or hearts.

---

## 🛠️ Features

- Say "no" in multiple **languages** (`en`, `de`)
- Say "no" in various **styles** (`sarcastic`, `shakespeare`, `corporate`, `http`, etc.)
- RESTful API design – easy to consume
- Can be used in frontend apps, Slack bots, browser extensions, or just when you're tired of saying it yourself
- Totally unnecessary, yet completely essential

---

## 🚀 Endpoints

### `GET /api/no`
Returns a random "no" (default language: English).

### `GET /api/no/{language}`
Returns a random "no" in the specified language.  
**Examples:**  
- `/api/no/de` → "Nö"
- `/api/no/en` → "Not in this live"

### `GET /api/no/style/{style}`
Returns a "no" in a specific style.  
**Supported styles:** `sarcastic`, `shakespeare`, `corporate`, `german`, `http`

### `GET /api/no/http`
Returns a meaningful HTTP-style "no" response like:
```json
{
  "message": "403 Forbidden – You shall not pass."
}
```

---

## 📦 Example Response

```json
{
  "message": "Absolutely not.",
  "language": "en",
  "style": "default"
}
```

---

## 🧠 Why tho?

Because your users, clients, friends, or enemies deserve more than just a boring "no".  
Let the API do the talking.

---

## 🧱 Tech Stack

- ASP.NET Core Web API
- C# (.NET 8 or later)
- Built-in randomness and sass

---

## 🧪 Running Locally

```bash
git clone https://github.com/docVoid/no-as-a-service.git
cd no-as-a-service
dotnet run
```

Navigate to:  
`http://localhost:5000/api/no`

Swagger UI:  
`http://localhost:5000/swagger`

---

## ✨ Contribution

Feel free to open a PR with:
- New languages (`no` in Swahili? Yes please!)
- New styles (Yoda-style, Pirate, Emo, etc.)
- Fun ideas, memes, or HTTP status messages

> 💬 Rule #1: Every PR must include at least one new way to say "no".

---

## 🧃 Sample Use Case

Need to say no in your Slack bot?

```js
fetch('https://no-as-a-service.pngrtz.com/api/no/style/sarcastic')
  .then(res => res.json())
  .then(data => console.log(data.message));
```

---

## 👥 Authors

Made with ❤️ and passive-aggression by:

- docVoid – Chief No Officer
- Robin – Senior Vice President of Denial

---

## 📄 License

MIT – You can do whatever you want, but don’t blame us if someone says no.

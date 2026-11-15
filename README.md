<p align="center">
  <img src="icons/simple-nutrition.png" width="64" alt="Simple nutrition">
  <img src="icons/budget-buddy.png" width="64" alt="Budget buddy">
  <img src="icons/football.png" width="64" alt="Football, not soccer">
  <img src="icons/stress-control.png" width="64" alt="Stress control">
</p>

<h1 align="center">Small apps, high standard</h1>

<p align="center">
  <b>One question. Your data. Nothing more.</b><br>
  Four mobile apps built from the same template – no login, no server, your data stays in the phone. In English and Swedish.
</p>

<p align="center">
  <a href="https://flyinggooner.github.io/"><b>Home page</b></a> ·
  <a href="https://flyinggooner.github.io/"><b>The presentation as a slideshow</b></a>
</p>

---

## 📱 The apps

| | App | The question it answers |
|:-:|---|---|
| <img src="icons/simple-nutrition.png" width="40" alt=""> | **[Simple nutrition](https://flyinggooner.github.io/simple-nutrition/)** | What have I eaten today – and how is my weight doing over time? |
| <img src="icons/budget-buddy.png" width="40" alt=""> | **[Budget buddy](https://flyinggooner.github.io/budget-buddy/)** | Does the month add up – and where does it get tight ahead? |
| <img src="icons/football.png" width="40" alt=""> | **[Football, not soccer](https://flyinggooner.github.io/Football-not-soccer/)** | What does the table look like, what is played next, how did my team do? |
| <img src="icons/stress-control.png" width="40" alt=""> | **[Stress control](https://flyinggooner.github.io/Stress-control/)** | What is spinning in my head – and what is the next step, so I can let it go? |

> **Install:** open the app in Chrome (Android) or Safari (iPhone) and choose *Install app* / *Add to Home Screen*. It then works offline. The first time, you choose English or Swedish.

---

## 💡 The starting point: most apps want too much

Account first. Notifications, ads, news, upsell. Your data on someone else's server. Features you never asked for.

- 🍽️ **The calorie app** has thousands of brand duplicates and a premium wall – when you only wanted to learn what the food contains.
- 💸 **The budget app** wants to connect to the bank and sort every coffee – when you only wanted to know if the month adds up.
- ⚽ **The football app** is full of news, betting and notifications – when you only wanted to see the table.

**These apps are the opposite: one question, one good answer, nothing more.**

---

## 🧭 Five principles

| | Principle | What it means |
|:-:|---|---|
| 🎯 | **One question per app** | Everything that does not help answer it is left out. |
| 🔒 | **Your data is yours** | It stays in the phone. No account, no server, no tracking. |
| ⚡ | **Quick in everyday life** | The most common things take a few seconds – the rest can be filled in later. |
| 🔍 | **Easy to trust** | Small code without dependencies, which can be read and tested. |
| 🔁 | **Better together** | What gets better in one app is brought into all of them. |

### 🎯 What is left out is just as important

Each app has a list of *non-goals* – things deliberately not built, however tempting they are.

| App | Deliberately left out |
|---|---|
| Simple nutrition | Brands, ready meals, micronutrients |
| Budget buddy | Bank connection, receipts for every purchase, tax calculation |
| Football, not soccer | News, squads, statistics, push notifications |
| Stress control | Sync, attachments, reminders via a server |
| **All** | **Account, server, ads, tracking** |

### 🧘 An app should remove stress, not create it

No notifications demanding attention. No streaks to lose. No red numbers shouting.

- **Write it down – let it go.** What has its next step written down does not need to spin in your head.
- **Habits before numbers.** Learn the ingredients; calories are there as support when you want.
- **Month, not receipt.** Plan the big things – the coffee does not need a line.

## 🛡️ Why this is the safer way

Sensitive data mostly leaks in two ways: **a company's database is hacked**, or **the company sells or shares it**. A budget app knows your whole financial life, a health app your weight and habits, a family app your children's names and worries.

| | Typical app with an account | These apps |
|---|---|---|
| Central database to hack | Yes – millions of users in one place | **None** – data only in your phone |
| Data sold or shared for ads/analytics | Common, even in paid apps | **Impossible** – no account, no analytics, requests out are blocked by the browser |
| Readable by staff or partners | Possible | **No** – only you have it |
| If the company shuts down | Your data goes with it | **Stays on your phone** |
| Backup | In the company's cloud | **Encrypted (AES-256) with your password** before it leaves the phone |

**Honestly:** nothing is 100 % safe. What remains is your own phone (lock it and keep it updated), a strong backup password, and trusting that the code on GitHub Pages is the open, reviewed code. But with no server there is nothing central to steal – for this kind of data that is as safe as a practical app gets.

---

## 🔒 Your data stays with you

- 🏠 **Only in the phone.** Everything is stored in the browser's storage on your device. There is no server to leak from.
- 🚫 **The browser keeps watch.** The page's security rules forbid requests out – even if the code wanted to, the browser would stop it.
- ⚖️ **Exceptions are reviewed.** The football app has to fetch results, but only from a single source, never with your data and only when you are looking.

---

## 🔑 Why the app asks for a password right away

> No account – but a key. The app is locked until you have chosen a password for your backup files.

- **It is not a login.** The password is sent nowhere and the app collects no data. It is just the key that locks your backup files.
- **No server will save you.** The data is only in the phone. If you lose it, or clear the browser, the backup file is all that is left.
- **Hence from the start.** If the password is chosen only when something has already gone wrong, it is too late. Chosen from the start, a backup is a single tap.
- **Already have a backup?** Restore it instead – the password that opens the file is saved.

### 💾 How the backup works

```
 1  Choose password      First start: "Create random password" (or your own).
         │               Save it in your password manager. The phone remembers it.
         ▼
 2  Save backup file     Settings → Data → Save backup file. One tap.
         │               Encrypted file – put it in the cloud, your email or on your computer.
         ▼
 3  Reminder             The app tells you every month.
         │
         ▼
 4  New phone            Restore backup file → password → summary → Replace.
                         Undo is available right afterwards.
```

### 🎲 How safe is the file?

The lock is **AES-256**, the same kind banks use, and every guess is slowed down: even one of the world's fastest graphics cards manages only ~10,000 guesses per second.

| Random characters | 1 graphics card | 1,000 graphics cards |
|---|---|---|
| 8 | 300 years | 4 months |
| 10 | 1 million years | 1,000 years |
| **16 (the app's)** | longer than the universe has existed | longer than the universe has existed |

> ⚠️ **Only if the characters are random.** Words, names and years are guessed first: `Summer2024!` has 11 characters but falls in a day.

**Smooth anyway:** the app remembers the password in the phone, so a backup takes one tap. The encryption protects the file when it *leaves* the phone – anyone who already has your unlocked phone sees everything in the app anyway. The password is never in the file, and without it the backup cannot be opened. Save it in your password manager.

<sub>The times are my own rough estimates: random letters and digits, PBKDF2 with 600,000 iterations.</sub>

---

## ✅ Tested before every version

| Step | What happens |
|:-:|---|
| **1 · Security check** | All code is searched for things that must not be there: code from outside, requests to unknown servers, unsafe storage. |
| **2 · Function tests** | The app is used in a real browser the way a person would: buttons are tapped, data is saved, backups are restored. |
| **3 · New version** | Only when everything is green does the app get a new version number. |
| **4 · Review** | Changes that affect security are reviewed separately before they are published. |

**Always checked:** only the app's own code runs · nothing leaves the phone · what you write is never shown as code · a changed backup file is not restored · what you save is exactly what you get back.

---

## 🧱 One template, four apps

1. A new app starts from a shared template – backup, theme, tests, help and language support are there from day one.
2. **Spec first:** idea, goals and what is deliberately not built.
3. Security is tested before the build and reviewed before upload.
4. What gets better in one app is brought back to the template – and out to all of them.

**The same foundation in all:** plain HTML, CSS and JavaScript · no frameworks or dependencies · no build step · works offline · Material Design 3 with its own key colour per app · light and dark theme · menu at the bottom for the thumb · the phone's Back closes one step at a time · built-in manual · English and Swedish.

---

<p align="center">
  <b>Small apps that do one thing well, keep your data with you and are tested before every version.</b><br>
  <a href="https://flyinggooner.github.io/">flyinggooner.github.io</a>
</p>

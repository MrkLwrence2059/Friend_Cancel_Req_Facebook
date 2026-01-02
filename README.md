# 🚫 Facebook – Auto Cancel Sent Friend Requests

A simple **manual browser-console script** to cancel all pending Facebook friend requests in one page load ⚡

> Works by clicking **Cancel request** buttons that are currently visible on screen 👀

---

## 🧰 Requirements

* 💻 PC or Laptop
* 🌐 **Brave Browser** (Chrome-based browsers also work)
* 🔐 Logged in to Facebook

---

## 🪜 How to Use (Step-by-Step)

1. 🌐 Open **Brave Browser**
2. 👉 Go to:

   **Facebook → Friends → Sent Requests**

   Or directly:

   ```
   https://www.facebook.com/friends/requests/?fcref=sent_requests
   ```
3. 📜 **Scroll down** until all requests you want to cancel are visible

   * Script runs **one time per page load**
4. ⌨️ Press:

   ```
   Ctrl + Shift + I
   ```
5. 🖥️ Go to the **Console** tab
6. ✍️ Type and press Enter:

   ```
   allow pasting
   ```
7. 📋 Paste the script below and press Enter

---

## 🧠 Script

```javascript
document.querySelectorAll('div[role="button"]').forEach(btn => {
  if (btn.innerText.trim() === 'Cancel request') {
    btn.click();
  }
});
```

---

## 🔁 Final Step

* 🔄 Refresh the page
* 🔁 Repeat if more requests exist

---

## ⚠️ Notes

* 👁️ Only cancels **visible** requests
* ⏳ Facebook may temporarily limit actions if abused
* 🧠 Use responsibly

---

## 📌 Disclaimer

This project is for **educational purposes only**. Use at your own risk ⚖️
Facebook UI changes may break the script.

---

## 👤 Author

**MrkLwrence2059** 🚀

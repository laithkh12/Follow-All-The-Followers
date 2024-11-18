# 📸 Instagram Follower Bot

<img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="instagram-logo" width="100"/>

A Python-based bot using **Selenium WebDriver** to automate Instagram account engagement by following the followers of a specific account. This tool is designed to help increase your account's visibility by engaging with users from similar niches.

---

## 📋 Features

- Logs in to Instagram automatically.
- Visits the followers list of a specified account.
- Scrolls through the followers list to load more users.
- Automatically follows users from the list.

---

## ⚙️ Prerequisites

Before you start, ensure you have the following:

1. **Python 3.7+**
2. **Google Chrome Browser**
3. **ChromeDriver** compatible with your Chrome version.
4. Install required Python libraries:
   ```bash
   pip install selenium
    ```
---
## 🚀 How to Use
1. Clone this repository or copy the script into your working directory.
2. Update the following variables in the script:
```python
SIMILAR_ACCOUNT = "buzzfeedtasty"  # Replace with the account to scrape followers from
USERNAME = "your_instagram_username"
PASSWORD = "your_instagram_password"
```
3. Run the script
---
## 📂 Script Workflow
1. Login to Instagram
  - Navigates to Instagram's login page.
  - Automatically enters credentials.
  - Handles cookie, save-login, and notification pop-ups.
2. Find Followers
  - Visits the followers list of a specified account.
  - Scrolls the list to load more followers.
3. Follow Users
  - Clicks the "Follow" button for each user in the list. 
  - Handles exceptions for already-followed users gracefully.
---
## 🖋️ Example Configuration
Update these variables in the script:
```python
SIMILAR_ACCOUNT = "example_account"  # Account to scrape followers from
USERNAME = "your_instagram_username"
PASSWORD = "your_instagram_password"
```
---
## ⚠️ Important Notes
- Account Security: Avoid using your primary Instagram account to reduce the risk of a ban.
- Avoid Spamming: Follow Instagram's guidelines to prevent account restrictions:
  - Avoid running the script multiple times a day.
  - Use realistic delays between actions.
- Dynamic Selectors: Instagram's HTML structure may change. Update the XPATHs or CSS Selectors if elements cannot be located.
---
## 🛠 Troubleshooting
- **Browser Not Opening**? Ensure the chromedriver executable is installed and added to your system's PATH.
- **Login Issues**? Verify your Instagram credentials and check for changes in Instagram's login process.
- **Buttons Not Clicking**? Update the XPATHs or CSS Selectors for the "Follow" buttons in the follow method.
---
## 🤝 Contributing
Contributions are welcome! Feel free to submit a pull request or suggest improvements.
--- 
## 📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
---
## 🌟 Acknowledgments
- Powered by Selenium WebDriver.
- Inspired by the need for simplified Instagram engagement.

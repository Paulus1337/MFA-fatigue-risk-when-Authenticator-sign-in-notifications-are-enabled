# How‑To: Keep Cloud Backup + keep MFA, but remove sign‑in notification approvals for sign‑in

This is a user‑side workaround. The goal is simple: stop “1FA tap approve to sign in” prompts from being a sign‑in method, while still keeping Microsoft Authenticator and Cloud Backup.

## Goal
Sign‑in should require:

1) **Password**
2) **Then a 6‑digit code** from Microsoft Authenticator

## Steps (high level)

1) In Microsoft Authenticator, enable **Cloud Backup** this will automatically setup Authenticators sign‑in notification.  
   ![Cloud-Backup](/assets/Cloud-Backup.png)
2) In your Microsoft account **Security** settings https://account.microsoft.com/security, open the page that lists your **sign‑in methods** (Manage how I sign in).
3) Remove the method that allows **sign‑in notification approvals** “Send sign‑in notification”.  
   ![Remove-Sign-in-Notification](/assets/Remove-Sign-in-Notification.png)
4) Add an authenticator method using **set up a different Authenticator app** (you can still use Microsoft Authenticator).  
   ![Setup-6code](/assets/Setup-6code.png)
5) Test sign‑in: it should ask for **password**, then the **6‑digit code**. Welcome to the 2FA club 🎉
   ![Success](/assets/Success.png)

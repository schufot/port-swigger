# [Lab: Basic clickjacking with CSRF token protection](https://portswigger.net/web-security/clickjacking/lab-basic-csrf-protected)

- Challenge information:
  - <img width="692" height="381" alt="image" src="https://github.com/user-attachments/assets/3e1e6f07-4125-4ce1-bee3-570540f8a4a9" />
- Solution:
- Explanation: Clickjacking
  - Malicious website is shown to a user with an overlaid layer using the CSS `z-index` property and an `opacity` of almost 0
  - This layer is what the user will actually interact with, when really they think they’re interacting with the visible, lower layer that looks like a legitimate website

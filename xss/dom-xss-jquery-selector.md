# [Lab: DOM XSS in jQuery selector sink using a hashchange event](https://portswigger.net/web-security/cross-site-scripting/dom-based/lab-jquery-selector-hash-change-event)

- Challenge information:
  - <img width="656" height="151" alt="image" src="https://github.com/user-attachments/assets/0ea0707c-8ead-43d6-95c6-daaef0dcd34f" />
- Solution:
  - <img width="1174" height="884" alt="image" src="https://github.com/user-attachments/assets/0c0041d5-5984-4d40-b55b-8942e7e6b59d" />
  - Website has an autoscroll implemented and we need to abuse that to make the browser execute the print() function
- Explanation:
  - DOM-based XSS attack: Malicious input will be passed to a sink that supports dynamic code execution through JQuery

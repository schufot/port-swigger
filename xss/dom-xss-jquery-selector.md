# [Lab: DOM XSS in jQuery selector sink using a hashchange event](https://portswigger.net/web-security/cross-site-scripting/dom-based/lab-jquery-selector-hash-change-event)

- Challenge information:
  - <img width="656" height="151" alt="image" src="https://github.com/user-attachments/assets/0ea0707c-8ead-43d6-95c6-daaef0dcd34f" />
- Solution:
  - <img width="1174" height="884" alt="image" src="https://github.com/user-attachments/assets/0c0041d5-5984-4d40-b55b-8942e7e6b59d" />
  - Website has an autoscroll implemented and we need to abuse that to make the browser execute the print() function
  - <img width="1174" height="884" alt="image" src="https://github.com/user-attachments/assets/6fcc34a3-8dec-45ed-90ba-4495544475d5" />
  - When clicking on "Store" and then "View exploit": <img width="1174" height="624" alt="image" src="https://github.com/user-attachments/assets/6ca86abd-7b72-4194-8611-3e9c2d5c6284" />
  - Then click "Deliver exploit to victim": <img width="1174" height="321" alt="image" src="https://github.com/user-attachments/assets/f4cadcf0-9271-4411-a9db-28d01bfef190" />


- Explanation:
  - DOM-based XSS attack: Malicious input will be passed to a sink that supports dynamic code execution through JQuery

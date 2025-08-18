# [Lab: Basic clickjacking with CSRF token protection](https://portswigger.net/web-security/clickjacking/lab-basic-csrf-protected)

- Challenge information:
  - <img width="692" height="381" alt="image" src="https://github.com/user-attachments/assets/3e1e6f07-4125-4ce1-bee3-570540f8a4a9" />
- Solution:
  - `<div>` will be visible to user, is the lower layer
  - `<iframe>` will be overlaid on the page, is the higher layer, this is the one the user actually clicks when they try to click the `div`
  - `<div>` and `<iframe>` need both their CSS: Make the iframe big enough to view te /my-account page items
  ```css
  <style>
  .visible {
      ... styles for the visible div that the user thinks they're interacting with
  }
  
  .overlaid-iframe {
      position:relative;
      width:700px;
      height: 700px;
      opacity: 0.1;
  }
  </style>
  ```
- Explanation: Clickjacking
  - Malicious website is shown to a user with an overlaid layer using the CSS `z-index` property and an `opacity` of almost 0
  - This layer is what the user will actually interact with, when really they think they’re interacting with the visible, lower layer that looks like a legitimate website

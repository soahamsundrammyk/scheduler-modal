# Premier Auto Deals – Dealership Website

A simple static website for a fictional car dealership, featuring a clean layout and a modal-based service scheduler embedded via an iframe.

---

## 🚗 Features

- Responsive layout with header, navigation, content, and footer
- "Schedule Service" option opens a **modal**, not a separate page
- Modal loads a third-party web app (e.g., appointment scheduler) using an `<iframe>`
- Seamless user experience with close functionality

---

## 🧪 Using the Modal (Schedule Service)

The modal is used instead of navigating away from the page. Here's how it works and how you can customize it:

### 🔧 How It Works

- The `<nav>` includes a `Schedule Service` link with an `id` of `scheduleLink`
- When clicked, it **opens a modal** by adding `display: block` to the `.modal` element
- Inside the modal is an `<iframe>` that loads a specific scheduling app URL
- A **close button (×)** in the corner allows users to exit the modal and return to the main page

---

### 🧩 Modal HTML Structure

```html
<!-- Modal -->
<div id="scheduleModal" class="modal">
  <div class="modal-content">
    <span class="close-button" id="closeModal">&times;</span>
    <iframe id="serviceIframe" src=""></iframe>
  </div>
</div>

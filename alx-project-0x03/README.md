# Reactify TS: Mastering Advanced TypeScript in React

This project demonstrates best practices and architecture in a Next.js TypeScript app, focusing on reusability and layout structuring using shared components (Header, Footer, Layout). It follows the DRY principle to reduce repetition and improve maintainability.

## 📁 Project Structure

- `/components/layouts/Header.tsx` – App header
- `/components/layouts/Footer.tsx` – App footer
- `/components/layouts/Layout.tsx` – Shared layout wrapper
- `/components/common/Button.tsx` – Reusable button
- `/interface/index.ts` - Centralized interfaces file

## 📦 Features

### 🏠 Landing Page with Imperative Routing

The landing page (`pages/index.tsx`) includes three main navigation buttons using **imperative routing** via `useRouter()` from `next/router`. Each button routes the user to a different mini app within the project:

- **Generate Text** ➝ `/generate-text-ai`
- **Text to Image** ➝ `/text-to-image`
- **Contact Us** ➝ `/counter-app`

This approach uses the reusable `Button` component with an `action` prop to handle routing behavior in a dynamic and scalable way.

![Landing page](./public/assets/images/landing_page.png)

### Custom 404 Page

- Created a user-friendly 404 error page with humorous messaging and a link back to home
- Located at: `pages/404.tsx`

![404 page](./public/assets/images/not_found_page.png)

## 🚀 Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```
2. Run the development server:
   ```bash
   npm run dev -- -p 3000
   ```
3. Access the app at: http://localhost:3000

## 📦 Packages Used

- react-icons/fa – Font Awesome icons as React components
- Next.js – React framework for production

## 🔧 Installation

```bash
npx create-next-app@latest alx-project-0x03 --typescript --eslint --tailwind
cd alx-project-0x03
npm install --save react-icons
```

## ✅ Additionals

- Montserrat font from Google Fonts applied globally in `styles/globals.css` using Tailwind CSS
  ```bash
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
  ```

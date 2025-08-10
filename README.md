This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.



## 🛠 Cách chạy local
```bash
npm install

# ✅ W0 – Checklist Khởi động & Chuẩn bị

## 1. Cài công cụ cần thiết
- [ ] Node.js 20 LTS (`node -v`, `npm -v`)
- [ ] Git (`git --version`)
- [ ] VS Code + Extensions: ESLint, Prettier, Tailwind CSS IntelliSense

## 2. Tạo 2 project local
- [ ] **Frontend (`web-user`)**: Next.js 14 + TypeScript + Tailwind + ESLint
- [ ] **Backend (`cms-admin`)**: Strapi (SQLite cho local)

## 3. Cấu hình Prettier & Gitignore
- [ ] `.prettierrc` với cấu hình `"singleQuote": true, "semi": false`
- [ ] `.prettierignore` thêm thư mục build/cache/env
- [ ] `.gitignore` ignore node_modules, build, .env, uploads (cho Strapi)

## 4. Tạo Brand mini-kit cho `web-user`
- [ ] Font: Plus Jakarta Sans (heading) + Inter (body)
- [ ] Màu chủ đạo: Gold `#C9A227`, Dark `#0F172A`, Link `#2563EB`
- [ ] Logo tạm: `public/logo.svg`

## 5. Tạo sitemap nháp
- [ ] File `SITEMAP.md` với cấu trúc: Home, About, Contact, Category, Tag, Post, Search, 404

## 6. Cấu hình biến môi trường local
- [ ] `web-user/.env`
  ```env
  NEXT_PUBLIC_SITE_URL=http://localhost:3000
  CMS_API_URL=http://localhost:1337

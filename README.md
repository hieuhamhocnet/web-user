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

# Web User (Next.js Frontend)

Frontend cho website/blog đa chủ đề.  
Tech stack: **Next.js 14 (App Router)**, **React 18**, **TypeScript**, **Tailwind CSS**, **shadcn/ui**.

## Mục tiêu
- Hiển thị bài viết theo danh mục và tag từ CMS (`cms-admin`).
- Hỗ trợ SEO mạnh (SSR/SSG/ISR, sitemap, meta tags, schema).
- Giao diện hiện đại, responsive, dễ đọc.
- Dễ bảo trì, dễ mở rộng chức năng trong tương lai.

## Công nghệ chính
- **Next.js 14 (App Router)** – render linh hoạt SSR/SSG/ISR.
- **Tailwind CSS** + **shadcn/ui** – xây dựng UI nhanh, tối ưu.
- **TypeScript** – code an toàn, dễ bảo trì.
- **next-sitemap** – tự sinh sitemap và robots.txt.
- **Supabase Storage/Cloudinary** – lưu trữ và tối ưu ảnh (tích hợp ở W1–W2).

## 🛠 Cách chạy local
```bash
npm install
npm run dev
# Mở http://localhost:3000
 Biến môi trường (.env)
env
Copy
Edit
NEXT_PUBLIC_SITE_URL=http://localhost:3000
CMS_API_URL=http://localhost:1337

 Cấu trúc thư mục chính
csharp
Copy
Edit
src/
  app/            # App Router pages/layout
  components/     # UI components tái sử dụng
public/           # Static assets (logo, favicon...)

🗺 Lộ trình phát triển
W0: Khởi động & chuẩn bị (đang thực hiện)
W1: Tích hợp CMS Strapi, lấy dữ liệu bài viết
W2: Hiển thị bài viết, phân trang, SEO cơ bản
W3: Tối ưu hiệu năng, SEO nâng cao
W4: Triển khai production

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

# CMS Admin (Strapi Backend)

Backend CMS cho website/blog đa chủ đề.  
Tech stack: **Strapi 4 (Node.js)**, **SQLite** (local), **PostgreSQL** (production), **REST/GraphQL API**.

## Mục tiêu
- Quản lý toàn bộ nội dung bài viết, danh mục, tag.
- Hỗ trợ soạn thảo bài với trình editor, upload ảnh.
- Phân quyền (Admin/Editor/Author) rõ ràng.
- Cung cấp API (REST & GraphQL) cho frontend (`web-user`).

## Công nghệ chính
- **Strapi 4** – CMS headless, dễ tuỳ biến.
- **Node.js 20** – môi trường runtime.
- **SQLite** – database cho local dev (nhanh, gọn).
- **PostgreSQL** – database cho môi trường production.
- **Supabase Storage/Cloudinary** – lưu trữ ảnh.

## 🛠 Cách chạy local
```bash
npm install
npm run develop
# Mở http://localhost:1337 (trang admin ở /admin)
Biến môi trường (.env)
Ví dụ local:

env
Copy
Edit
APP_KEYS=changeme1,changeme2,changeme3,changeme4
API_TOKEN_SALT=changeme
ADMIN_JWT_SECRET=changeme
JWT_SECRET=changeme
Khi deploy production, các giá trị trên phải được thay bằng secret an toàn.

Cấu trúc thư mục chính
bash
Copy
Edit
config/          # Cấu hình server, middleware, plugin
database/        # Migrations và seeds
src/
  api/           # Content Types & Controllers
  extensions/    # Tuỳ chỉnh plugin
public/uploads/  # Ảnh upload local (nên ignore trong Git)

🗺 Lộ trình phát triển
W0: Khởi động & chuẩn bị (đang thực hiện)
W1: Tạo Content Types (Post, Category, Tag), mở public API, cấu hình CORS
W2: Tích hợp với web-user, kiểm thử CRUD bài viết
W3: Tối ưu query, phân quyền nâng cao
W4: Deploy production + backup & monitoring

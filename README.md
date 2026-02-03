# PixPilot-SaaS

🚀 **Build Cloudinary AI Powered SaaS**

This full-stack SaaS helps creators upload, compress, transform, and optimize video content with Cloudinary’s media APIs. The platform pairs a modern UI with secure auth, reliable storage, and fast media delivery.

## 📌 Overview

The app offers streamlined uploads, AI-driven transformations, and a polished dashboard experience. Video assets are stored and processed in Cloudinary, while Prisma + NeonDB handle persistence. Everything is wired together with TypeScript-first tooling and shipped via Vercel.

## ✨ Features

- 📤 Video uploading with progress feedback
- 🗜️ AI-assisted compression and optimization
- ⚙️ Configurable Cloudinary transformations
- 💾 NeonDB + Prisma-backed storage
- 🔐 Optional Clerk or NextAuth authentication
- 🎨 TailwindCSS + DaisyUI interface
- 📁 Dashboard with upload history
- 📥 Downloadable optimized assets
- 🌐 Ready for Vercel deployment

## 🛠️ Tech Stack

**Frontend**
- Next.js 14 (App Router)
- React
- TailwindCSS
- DaisyUI

**Backend / Services**
- Cloudinary (video compression + storage)
- Prisma ORM
- NeonDB (PostgreSQL serverless)

**Tooling**
- TypeScript
- ESLint / Prettier
- Vercel deployment

## 📂 Project Structure

```
├── app/
│   ├── (app)/
│   │   ├── layout.tsx
│   │   ├── home/page.tsx
│   │   ├── social-share/page.tsx
│   │   └── video-upload/page.tsx
│   ├── (auth)/sign-in/[[...sign-in]]/page.tsx
│   ├── (auth)/sign-up/[[...sign-up]]/page.tsx
│   ├── api/
│   │   ├── image-upload/route.ts
│   │   ├── video-upload/route.ts
│   │   └── videos/route.ts
│   ├── layout.tsx
│   └── page.tsx
├── components/VideoCard.tsx
├── prisma/
│   ├── migrations/
│   └── schema.prisma
├── public/
├── types/index.ts
├── middleware.ts
├── next.config.mjs
├── package.json
├── tailwind.config.ts
├── tsconfig.json
└── README.md
```

## 🚀 Getting Started

1️⃣ **Clone the repository**

```powershell
git clone https://github.com/aryannnpatil/PixPilot-saas-nextjs.git
cd PixPilot-saas-nextjs
```

2️⃣ **Install dependencies**

```powershell
npm install
```

3️⃣ **Configure environment variables**

Create a `.env` file:

```bash
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

DATABASE_URL=

NEXT_PUBLIC_SITE_URL=http://localhost:3000
```

4️⃣ **Push Prisma schema**

```powershell
npx prisma migrate dev
```

5️⃣ **Run the development server**

```powershell
npm run dev
```

## 🧠 Cloudinary Transformations

PixPilot leverages Cloudinary’s APIs for:
- Video compression
- Format conversion
- Resolution reduction
- Adaptive bitrate streaming
- AI-powered tuning such as `q_auto` and `f_auto`

## 🛑 Requirements

- Node.js 18+
- Cloudinary account
- NeonDB PostgreSQL database
- Git + npm

## 📸 Screenshots *(optional)*

Add screenshots when ready:

```
![Dashboard](./public/dashboard.png)
![Upload Page](./public/upload.png)
```

## 📜 License

Released under the MIT License.

## 🤝 Contributing

Contributions are welcome—fork the repo and open a PR.

## ⭐ Support

If this project helps you, a star ⭐ on GitHub goes a long way!

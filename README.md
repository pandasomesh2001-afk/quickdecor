# QUICK DECOR — Full Stack Website

Brand: **THE BOY'S EVENTS AND CATERES presents QUICK DECOR**  
Theme: Premium black, gold, and white event decoration booking website.  
Stack: **Next.js 14 + MongoDB + NextAuth + Cloudinary + Tailwind CSS**

## Features

- Responsive premium public website
- Category pages for decoration services
- Setup/package detail pages with gallery slider
- Booking inquiry form with auto-selected category/setup
- Admin login panel
- Admin dashboard analytics
- Manage booking inquiries
- Manage categories
- Manage setup packages
- Manage settings/social/contact details
- Cloudinary image upload API
- MongoDB database models

## Run Locally

```bash
npm install
cp .env.example .env.local
npm run dev
```

Open: `http://localhost:3000`

## First Setup

1. Create MongoDB database and add `MONGODB_URI` in `.env.local`.
2. Add a long random `NEXTAUTH_SECRET`.
3. Add Cloudinary keys if you want admin image upload.
4. Start project using `npm run dev`.
5. Visit this URL one time to create default admin and categories:

```text
http://localhost:3000/api/seed
```

Default admin comes from `.env.local`:

```env
ADMIN_EMAIL=admin@quickdecor.in
ADMIN_PASSWORD=Admin@123
```

## Upload to GitHub

```bash
git init
git add .
git commit -m "Initial Quick Decor project"
git branch -M main
git remote add origin YOUR_GITHUB_REPO_URL
git push -u origin main
```

## Deploy

Recommended: Vercel + MongoDB Atlas + Cloudinary.
Add the same `.env.local` values in Vercel Environment Variables.

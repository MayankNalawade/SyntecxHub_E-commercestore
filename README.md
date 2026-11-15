# SyntecxShop – E-Commerce Store (Project 1)

A single-page e-commerce app covering the project brief:

- Product listings with search and category filters
- Shopping cart and checkout (demo payment)
- User registration/login with JWT-style tokens and role-based authorization
- Admin dashboard: manage products, stock, and order status
- Production-ready static deployment

## Run locally
Open `index.html` in a browser, or serve the folder:

    npx serve .

## Demo accounts
- Admin: admin@shop.com / admin123
- Customers: register from the Login page

## Deploy
- Netlify: drag and drop this folder at app.netlify.com/drop (netlify.toml included)
- Vercel: `npx vercel --prod` (vercel.json included)
- GitHub Pages: push to a repo, then Settings > Pages > deploy from main branch

## Important note
This version runs fully in the browser: data is stored in localStorage and the JWT
is signed client-side, so it is a demo. For real production use, move auth, data,
and payments to a backend:

| Layer    | Suggested stack                          |
|----------|------------------------------------------|
| Backend  | Node + Express (or Django / FastAPI)     |
| Database | MongoDB or PostgreSQL                    |
| Auth     | bcrypt + jsonwebtoken (server-side secret) |
| Payments | Stripe or Razorpay                       |

## Structure
    index.html      the whole app (HTML, CSS, JS)
    netlify.toml    Netlify config
    vercel.json     Vercel config
    README.md       this file

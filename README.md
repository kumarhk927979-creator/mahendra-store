# Mahendra General Store — Paliganj

Paliganj ka online grocery store website. Fruits/sabzi/dairy hata kar jo catalogue hai uske saath,
plus WhatsApp par order, cart, offers aur installable app (PWA) support.

## Files

| File | Kaam |
|------|------|
| `index.html` | Home page (categories, offers, bestsellers) |
| `products.html` | Poora catalogue — search + category filter + cart |
| `about.html` | Store ke baare me |
| `contact.html` | Contact + WhatsApp order form + map |
| `manifest.json` | App info (installable app ke liye) |
| `sw.js` | Service worker (offline support) |
| `icon-192.png`, `icon-512.png` | App icons |
| `.nojekyll` | GitHub Pages ko batata hai ki Jekyll skip kare |

Saare paths relative hain, isliye site kisi bhi folder/subpath me chal jaati hai.

## GitHub Pages par live kaise karein

1. github.com par apna account banayein / login karein.
2. Upar right me **+** → **New repository**.
3. Repository name: `mahendra-store` (ya jo chahein). Visibility: **Public**. **Create repository**.
4. Naye repo me **Add file → Upload files** par jaayein.
5. Is folder ki **saari files** (README.md, index.html, products.html, about.html,
   contact.html, manifest.json, sw.js, icon-192.png, icon-512.png, .nojekyll) select karke
   drag-and-drop karein → neeche **Commit changes**.
6. Repo me **Settings → Pages** kholein.
7. "Build and deployment" me Source = **Deploy from a branch**; Branch = **main**, folder = **/ (root)** → **Save**.
8. 1-2 minute baad aapka link ready hoga:
   `https://<aapka-username>.github.io/mahendra-store/`

Bas! Ye link WhatsApp par share kar dein. Phone par kholne par "Install App" bhi aa jaayega.

## Note

- App install (PWA) feature sirf HTTPS par chalta hai — GitHub Pages free HTTPS deta hai.
- Products, prices aur offers badalne ke liye seedha `products.html` me data edit karein
  (file ke `<script>` ke andar `const PRODUCTS = [...]` wala hissa).
- Prices indicative hain — asli daam apne hisaab se set karein.

# ovro.ja

বাংলাদেশ-কেন্দ্রিক ovro.ja storefront frontend.

## Cloudflare Pages deployment

এই repository-তে framework/build pipeline নেই; root directory-তে সরাসরি `index.html` আছে।

1. Cloudflare Dashboard → **Workers & Pages** → **Create application** → **Pages**।
2. **Import an existing Git repository** নির্বাচন করে GitHub repository `jovibebd-hub/ovro.ja` connect করুন।
3. Production branch: `main`
4. Framework preset: **None**
5. Build command: `exit 0`
6. Build output directory: `.`
7. Save and Deploy চাপুন।

সফল deployment-এর পর Cloudflare `*.pages.dev` URL দেবে। Git integration থাকলে `main`-এ পরবর্তী commit push করলেই redeploy হবে।

## বর্তমান কোডে যা আছে

- Responsive Bengali storefront layout
- Product search ও category filter
- Product detail dialog
- Browser-local cart (একই browser-এ cart সংরক্ষিত থাকে)
- ১০টি প্রাথমিক demo catalogue item

## এখনো production-ready নয়

- Product image gallery/zoom এবং যাচাইকৃত product photography
- Verified sale price, variants, supplier-confirmed stock
- Checkout, order database/API, customer order tracking
- Admin authentication/dashboard ও product management
- Payment gateway, delivery integration, email/SMS notifications
- Published contact details, return/shipping/privacy policies

দাম/স্টক/পেমেন্ট বা ব্যবসায়িক তথ্য অনুমান করে দেখানো হয়নি। এগুলো যুক্ত না হওয়া পর্যন্ত সাইটটি frontend preview/catalogue হিসেবে ব্যবহার করুন; live order নেওয়ার জন্য প্রস্তুত নয়।

এই repository, sheet এবং brand আলাদা ovro.ja-এর জন্য; JO Vibe-এর project-এর সঙ্গে মেশানো নয়।

# راهنمای انتشار «همیار ساختمان» در Google Play

## ۱) میزبانی (HTTPS اجباری)
همهٔ فایل‌های این پوشه را روی یک دامنهٔ HTTPS آپلود کنید (Netlify / Cloudflare Pages / GitHub Pages). InfinityFree برای TWA مناسب نیست.
در Supabase ← Authentication ← URL Configuration: آدرس سایت را در Site URL و Redirect URLs وارد کنید (برای تأیید ایمیل و بازیابی رمز).

## ۲) ساخت فایل AAB
1. به pwabuilder.com بروید، آدرس سایت را بدهید ← Package for stores ← Android.
2. Package ID: com.hamyar.sakhteman ، نام: همیار ساختمان.
3. فایل signing key را بسازید و **حتماً نگه دارید** (رمز و فایل .keystore).
4. فایل .aab را دانلود کنید.

## ۳) Digital Asset Links
SHA-256 کلید امضا (Play Console ← App integrity) را در `.well-known/assetlinks.json` جایگزین کنید و فایل را روی دامنه بگذارید: `https://دامنه/.well-known/assetlinks.json` تا نوار آدرس مرورگر در برنامه حذف شود.

## ۴) Play Console
- حساب توسعه‌دهنده (۲۵ دلار) ؛ ساخت برنامه ← آپلود AAB.
- آدرس Privacy Policy: `https://دامنه/privacy.html`
- بخش Account deletion: آدرس برنامه + مسیر «پنل من ← حذف حساب کاربری».
- Data safety: جمع‌آوری ایمیل، نام، تلفن، آدرس، تصویر رسید؛ رمزگذاری در انتقال: بله؛ امکان حذف: بله؛ فروش داده: خیر.
- دسته: House & Home. رده‌بندی سنی: همه.
- تصاویر: آیکن ۵۱۲ (در icons/)، Feature graphic ۱۰۲۴×۵۰۰، حداقل ۲ اسکرین‌شات.
- برای حساب شخصی جدید: تست بسته با ۱۲ تستر به مدت ۱۴ روز لازم است.

## ۵) توضیح کوتاه فروشگاه
ثبت درخواست تعمیرات ساختمان در گرگان، دیدن متخصص تأییدشدهٔ محله و پیگیری شفاف کار تا تحویل.
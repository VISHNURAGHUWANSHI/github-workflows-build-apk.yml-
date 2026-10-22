# Durga Pooja Hisab — Capacitor (Android APK)

Chanda (income) + kharch (expense) + rasid billing app. App ka poora code `www/index.html` me hai.

## Tareeka 1: Bina kuch install kiye APK (GitHub se)
1. github.com par free account banayein aur naya repository banayein.
2. Is folder ki saari files (hidden `.github` folder ke saath) us repo me upload karein.
3. Repo me **Actions** tab kholein -> **Build APK** -> **Run workflow**.
4. 5-8 minute baad run ke andar **Artifacts** se `durga-pooja-hisab-apk` download karein.
5. Zip kholkar `app-debug.apk` phone me bhejein aur install karein (Settings me "Install unknown apps" allow karna hoga).

## Tareeka 2: Apne computer par
Zaroori: Node.js 18+, JDK 17, Android Studio (SDK ke saath).
```
npm install
npm run setup     # android folder banayega
npm run apk       # APK: android/app/build/outputs/apk/debug/app-debug.apk
```
Ya `npm run open` se Android Studio me kholein aur Run dabayein.

## App me badlav karne ke baad
`www/index.html` edit karein, phir `npm run sync` (ya Tareeka 1 me dubara push).

## Play Store ke liye
Debug APK sirf install/testing ke liye hai. Play Store ke liye Android Studio me
Build > Generate Signed Bundle / APK se signed release banayein.

## Dhyan rakhein
- Data phone ke andar save hota hai. App uninstall ya "Clear data" par hat jayega; Report se CSV backup lete rahein.
- Rasid "Share / WhatsApp" se bhejein. Android app me Print/PDF button nahi dikhta.

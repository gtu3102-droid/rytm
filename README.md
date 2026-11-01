# رتم — بناء ملف APK

1. أنشئ مستودعًا جديدًا (خاصًا أو عامًا) على github.com وارفع كل محتويات هذا المجلد إليه (بما فيها مجلد .github).
2. افتح تبويب **Actions** ثم **Build Android APK** ثم **Run workflow** (يعمل تلقائيًا أيضًا عند الرفع).
3. بعد دقائق قليلة نزّل الملف **rytm-apk** من قسم Artifacts، وفكّ الضغط لتجد app-debug.apk.
4. انقله إلى الجوال وثبّته (فعّل «التثبيت من مصادر غير معروفة»).

للبناء المحلي: npm install && npx cap add android && npx capacitor-assets generate --android && npx cap sync android && cd android && ./gradlew assembleDebug

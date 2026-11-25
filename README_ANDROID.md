# Aplikant Duel — Android (Google Play)

Loyiha Capacitor 8 asosida tayyorlangan. O'yinning o'zi `www/` papkasida (index.html + questions.json).

## Build qilish
1. Android Studio (eng so'nggi versiya) va Node.js 20+ o'rnating.
2. Papkada: `npm install`, keyin `npx cap sync android`.
3. `npx cap open android` — loyiha Android Studio'da ochiladi.
4. Build > Generate Signed App Bundle / APK > Android App Bundle. Yangi keystore yarating va uni xavfsiz joyda saqlang (yo'qolsa, ilovani yangilab bo'lmaydi).
5. Natija: `android/app/release/app-release.aab`.

## Google Play
1. play.google.com/console — dasturchi akkaunti (bir martalik to'lov).
2. Create app → nom: Aplikant Duel; til; App/Game: Game; Free.
3. Store listing: qisqa tavsif, to'liq tavsif, ikonka 512×512 (`play_icon_512.png`), feature graphic 1024×500, kamida 2 ta skrinshot.
4. App content: Privacy policy URL, Data safety (ilova hozircha ma'lumot to'plamaydi, faqat qurilmada saqlaydi), Content rating anketasi, Target audience 18+.
5. Testing → Closed testing (yangi shaxsiy akkauntlar uchun 12 ta tester, 14 kun) → Production.

## Savollarni yangilash
`www/questions.json` ni almashtiring va `npx cap sync android` qiling. versionCode'ni `android/app/build.gradle` da oshiring.

# הנחיות ל-Claude

## על הפרויקט
- משחק דפדפן תלת־ממדי בקובץ אחד: `game3d_v3.html` (three.js r128 מ-CDN). פרטי המשחק והמקשים נמצאים ב-`README.md`, אותו קוראים ראשון.
- `index.html` רק מפנה ל-`game3d_v3.html`.

## GitHub
- החשבון: `bigi4ever`, ה-repository: `bigi4ever/gun-game` (ציבורי).
- GitHub Pages מופעל (Deploy from a branch, `main`, `/ (root)`). המשחק באוויר בכתובת https://bigi4ever.github.io/gun-game/ ומתעדכן אוטומטית דקה-שתיים אחרי כל push ל-`main`.
- סטטוס הפרסום אפשר לבדוק עם `gh api repos/bigi4ever/gun-game/actions/runs` (ה-workflow "pages build and deployment"). בסביבת הענן אין גישה ישירה ל-`github.io`.

## איך לעבוד
- לשמור שינויים ישר ל-`main`, בלי ליצור ענפים, אחרי שבדקתם שהמשחק עובד.
- לבדוק כל שינוי בדפדפן (Playwright עם Chromium) ולוודא שאין שגיאות בקונסול. בסביבת הענן ה-CDN של three.js חסום, אז טוענים עותק מקומי (`npm i three@0.128.0`) דרך `page.route`.
- לעדכן את `README.md` כשמשנים התנהגות של המשחק.
- המשתמש מתחיל: להסביר צעדים ב-GitHub בפשטות ובעברית.

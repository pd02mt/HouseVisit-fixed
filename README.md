# לומדת ביקור בית — React + Vite

הפרויקט נבנה לפי תוכן ומסכים מתוך קובץ ה-PDF שסופק (ייצוא של העיצוב). קובץ Figma המקורי לא צורף, ולכן ניתן לדייק את העיצוב עוד יותר אם יימסר קישור/ייצוא מתאים.

## הפעלה ב-VS Code
1. חלצי את תיקיית הפרויקט.
2. פתחי את התיקייה ב-VS Code.
3. אם Node.js מותקן והתלויות כבר זמינות במחשב: הריצי `npm install` פעם אחת, ואז `npm run dev`.
4. לפתיחת גרסת בנייה: `npm run build`.

## מחשב ללא אינטרנט
- פתחי את `offline.html` בדפדפן ישירות, בלי שרת ובלי התקנות. הוא משתמש רק בקבצים מקומיים שבתיקייה.
- סביבת Vite עצמה אינה דורשת אינטרנט בזמן ההרצה, אבל התקנת React/Vite הראשונית דורשת תלויות מקומיות או העתקה ממחשב אחר. לכן גרסת `offline.html` כלולה להפעלה מיידית ללא רשת.

## מה כלול
- 15 שאלות אינטראקטיביות בעברית ובכיווניות RTL.
- בדיקת תשובה, סימון נכון/לא נכון ומשוב מקצועי.
- כפתור מעבר לשאלה הבאה, פס התקדמות ומסך סיום עם ניקוד.
- תמונות מקומיות שחולצו מה-PDF; אין שימוש ב-CDN או קריאות רשת בזמן ההפעלה.

## GitHub Pages deployment

This project is configured for a repository named `HouseVisit` and uses Vite's `/HouseVisit/` base path. If your repository name differs, update `base` in `vite.config.js` to `/<repository-name>/`.

1. Upload/commit the project files to the repository's `main` or `master` branch. Do not upload `node_modules`.
2. In GitHub, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
3. The workflow at `.github/workflows/deploy.yml` builds the project and deploys `dist` after a push to `main` or `master`.
4. Open the repository's **Actions** tab and check that **Deploy HouseVisit to GitHub Pages** completes successfully.

To test locally, run `npm install`, then `npm run dev`. To build, run `npm run build`.


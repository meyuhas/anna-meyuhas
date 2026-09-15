# anna-meyuhas.com - ניווט

מפת הפרויקט. **הכללים יושבים ב-`CLAUDE.md` - לקרוא אותו לפני עריכה.** המסמך הזה הוא המפה: איפה כל דבר נמצא.

**מיקום:** `~/GitHub/anna-meyuhas` · **גודל:** 6.8 MB · **ענף:** `main`
**ריפו:** `github.com/meyuhas/anna-meyuhas` · **חי:** https://anna-meyuhas.com
**קומיט אחרון:** 09/08/26 - הירו: גובה מצומצם וכפתור בולט לאודות
**סוג:** אתר סטטי. אין `package.json`, אין build. נטליפיי מגישה את התיקייה כמו שהיא.

---

## מפת קבצים

```
index.html          859 שורות · 108K   דף הבית. רכיב x-dc יחיד, הלוגיקה בתחתית
support.js        1,911 שורות         ספריית הרנדור · לא נוגעים
netlify.toml                          publish="." · cache לאיורים · security headers
CLAUDE.md                             כללי עבודה · קול · מלכודות
README.md                             סקירה קצרה
accessibility.html                    הצהרת נגישות
thanks.html                           עמוד תודה לטופס
sitemap.xml · robots.txt              SEO
og-image.jpg                          תמונת שיתוף
favicon.png · favicon-512.png · apple-touch-icon.png
```

### `articles/` - חמישה מאמרים, כל אחד עמוד עצמאי
```
about-therapy.html
leadership-and-career.html
making-decisions.html
self-reliance-and-burnout.html
therapeutic-relationship.html
```

### `illustrations/` - 20 איורי אקוורל ב-WebP
```
hero · about · palette · recognition · testimonials
clinic-pt · clinic-ta · clinic-zoom          שלושת ערוצי הטיפול
icon-1 … icon-5                              אייקוני סקשנים
tool-1 … tool-6                              כלים טיפוליים
soft-wash                                    טקסטורת רקע
```
נטליפיי מגישה אותם עם `max-age=31536000, immutable` - **שם קובץ שמתחלף מחייב שינוי בהפניה, אין invalidation.**

---

## עוגני הדף · `index.html`

לפי סדר הופעה. אלה גם יעדי הניווט בתפריט.

| עוגן | הסקשן |
|------|-------|
| `#top` | ראש הדף · הירו |
| `#about` | אודות |
| `#invited` | למי זה מיועד |
| `#recognition` | זיהוי · הדפוסים |
| `#palette` | פלטת הכלים |
| `#workshops` | סדנאות |
| `#articles` | מאמרים · `#art-body-0` … `#art-body-4` |
| `#testimonials` | המלצות |
| `#where` | איפה · מפת הקליניקה |
| `#booking` | קביעת פגישה · Calendly |
| `#writeme` | כתבי לי |
| `#main` | עוטף התוכן |
| `#mobile-menu` | תפריט נייד |

**שדות טפסים:**
`#cf-name` `#cf-contact` `#cf-msg` - טופס `contact`
`#wl-name` `#wl-contact` `#wl-note` - טופס `waitlist`

---

## שירותים

| מה | איפה |
|----|------|
| אחסון | Netlify, פרויקט `anna-meyuhas`, מחובר לגיטהאב |
| טפסים | Netlify Forms - `contact` ו-`waitlist`, התראות למייל |
| יומן | Calendly - https://calendly.com/meyuhastv/30min |
| דומיין | Porkbun, ALIAS ל-`apex-loadbalancer.netlify.com` |
| קליניקה | ב.ס.ר סיטי, ז'בוטינסקי 61 פתח תקווה · `32.0918374, 34.8600663` |

---

## פרסום

```bash
cd ~/GitHub/anna-meyuhas
git push origin main
# נטליפיי בונה 30-60 שניות
curl -s https://anna-meyuhas.com | grep <מחרוזת>
```

---

## חמש מלכודות · מתוך `CLAUDE.md`

1. **התוכן מרונדר מראש.** לולאות `sc-for` הורחבו ל-HTML סטטי. המערכים ב-`renderVals` נשארו כקוד מת - טקסט שמופיע בשניהם חייב עדכון בשני המקומות.
2. **הרנדרר משמיט את `hidden`.** להסתרה - `style` מוטבע.
3. **אין להחזיק את הריפו בדרופבוקס.** הסנכרון נועל את `.git`.
4. **מיקוד בשאילתת מפה מסיט את הסיכה.** קואורדינטות מפורשות בלבד.
5. **בדיקת ה-HTML הגולמי לא מספיקה.** יש פער בין המקור לתוצר הרנדרר - לאמת בדפדפן ובנייד.

---

## קול

עברית בגובה העיניים, פנייה בלשון נקבה, בלי סופרלטיבים ובלי שפה שיווקית. הטקסטים נכתבו בקול של אנה.

**מקפים:** מקף רגיל `-` בלבד. יוצא דופן: המקף העברי `־` באיות תקני - "גופנית־נפשית", "גוף־נפש".

     1|---
     2|name: seedance-15sec-technique
     3|description: >
     4|  Use this skill when the user wants to create a video LONGER than 15 seconds with Seedance 2.0,
     5|  wants full continuity across multiple clips, or asks about "שיטת ה-15 שניות" / "video extend" /
     6|  "המשכיות" / "סרטון ארוך". Also load this skill as a complement to seedance-prompt-master
     7|  when the user confirms they want the 15-second technique.
     8|---
     9|
    10|# שיטת ה-15 שניות — Seedance 2.0 Video Extend
    11|
    12|**גילוי: דניאל ביטון** — איש קולנוע שבילה לילה שלם בניסויים עד שפיצח את זה.
    13|**שודרג עם שיטת Golden Angel** — הדרך הנכונה לשרשר קליפים ברמה סינמטית.
    14|
    15|## הרעיון
    16|
    17|Seedance 2.0 מוגבל ל-15 שניות לקליפ. אבל אם מעלים קליפ גמור בחזרה כ-reference video
    18|ומכתיבים המשך — הוא **ממשיך בדיוק מאיפה שנעצר**. לא "קליפ דומה". ממש המשך.
    19|
    20|למה? כי Seedance מנתח **כל המסלול** — כיוון מצלמה, תאורה, קומפוזיציה, קצב תנועה.
    21|
    22|---
    23|
    24|## שלב 1 — תכנון camera handoff לפני הגנרציה
    25|
    26|**החדשה מ-Golden Angel:** לפני שמייצרים קליפ 1, תכנן את ה-end position של כל קליפ.
    27|
    28|```
    29|קליפ 1: Start [A] → End [B]
    30|קליפ 2: Start [B] → End [C]
    31|קליפ 3: Start [C] → End [D]
    32|```
    33|
    34|**דוגמה אמיתית מ-Golden Angel:**
    35|```
    36|קליפ 1: Start low-angle right side → End high-angle left profile
    37|קליפ 2: Start high-angle left profile → End stabilized handheld
    38|קליפ 3: Start stabilized handheld → End slightly below, unstable framing
    39|```
    40|
    41|זה עיקרון אחד, והוא מה שגורם לוידאו להרגיש כמו single take ארוך.
    42|
    43|---
    44|
    45|## שלב 2 — הקליפ הבסיסי (15 שניות ראשונות)
    46|
    47|**מה שחובה בפרומפט הראשון:**
    48|- Core Theme מדויק — ז'אנר + אסתטיקה + מצב נרטיבי
    49|- Visual Style Lock — תעתיק בדיוק בכל קליפ
    50|- Camera Rules — Single continuous take + end position מתוכנן
    51|- 5 בלוקים × 3 שניות (0-3, 3-6, 6-9, 9-12, 12-15)
    52|- End State — מה לא נפתר
    53|- Finish Lock — same spec + רשימת NOT
    54|
    55|---
    56|
    57|## שלב 3 — ההעלאה מחדש (הקסם)
    58|
    59|1. הורד את הקליפ שנוצר
    60|2. עלה אותו ל-Seedance כ-**reference video** (`@video`)
    61|3. כתוב פרומפט המשך עם שורת continuity
    62|4. בחר 15 שניות נוספות
    63|5. לחץ Generate
    64|
    65|---
    66|
    67|## שלב 4 — פרומפט ההמשך
    68|
    69|### ❌ טעות — לתאר מחדש מה שכבר קרה:
    70|```
    71|"a warrior standing in ruins" ← המודל יתחיל מחדש
    72|```
    73|
    74|### ✅ נכון — שורת continuity + רק מה קורה הלאה:
    75|```
    76|Continue the story and scene showing in @video, and maintain all aspects of continuity,
    77|following this prompt:
    78|
    79|Core Theme: [אותו ז'אנר], [אותה אסתטיקה], [מצב נרטיבי חדש], [אותה סביבה]
    80|
    81|Character Setup
    82|[עדכון מינימלי לבגד/מצב — לא לכתוב מחדש הכל]
    83|
    84|Visual Style
    85|[העתק מדויק מקליפ 1]
    86|
    87|Camera Rules
    88|Single continuous take
    89|Continue from [end position של קליפ הקודם], [מסלול חדש], end [position חדש]
    90|Subtle handheld "breathing" motion throughout
    91|
    92|[5 בלוקים × 3 שניות]
    93|
    94|End State
    95|[מה עדיין לא נפתר]
    96|
    97|Finish
    98|Same [spec] — זהה
    99|```
   100|
   101|---
   102|
   103|## הטכניקה של Finish Lock — המנוע לעקביות
   104|
   105|**החדשה מ-Golden Angel:** כל קליפ מסתיים ב-Finish block זהה.
   106|
   107|```
   108|Finish
   109|Same IMAX simulation, Panavision 35mm f4
   110|Same [palette שלך], compressed shadows, film grain
   111|No added glow beyond original system
   112|No [heroic pose / beautification / fantasy softness]
   113|Everything remains [מילת הטון שלך]
   114|```
   115|
   116|**למה זה עובד:** הוא משמש כ-consistency anchor. Seedance רואה שאתה לא רוצה drift.
   117|
   118|---
   119|
   120|## שרשור
   121|
   122|```
   123|קליפ 1 (15") → reference ← קליפ 2 (15") → reference ← קליפ 3...
   124|```
   125|
   126|| זמן רצוי | מספר סבבים |
   127||-----------|------------|
   128|| 30 שניות | 2 |
   129|| 45 שניות | 3 |
   130|| דקה | 4 |
   131|| דקה וחצי | 6 |
   132|| ∞ | ∞ |
   133|
   134|---
   135|
   136|## 5 טיפים חובה מהשטח
   137|
   138|**טיפ 1 — תמיד 15 שניות**
   139|קליפ קצר לא נותן מספיק context. 15 שניות = המקסימום = הכי טוב.
   140|
   141|**טיפ 2 — Camera Handoff מתוכנן**
   142|קבע לפני הגנרציה מה ה-end position של כל קליפ. כתוב אותו ב-Camera Rules.
   143|
   144|**טיפ 3 — Visual Style Lock זהה בדיוק**
   145|העתק בדיוק — אותן מילים, אותן מפרט, אותה סדר. שום שינוי.
   146|
   147|**טיפ 4 — Finish Block בכל קליפ**
   148|כולל הרשימה השלילית (no glow / no heroic / etc.). זה ה-anchor.
   149|
   150|**טיפ 5 — "avoid static shots"**
   151|הוסף לכל פרומפט. שינוי קטן, שיפור עצום.
   152|
   153|---
   154|
   155|## הטעויות שחייבים להימנע
   156|
   157|| טעות | תוצאה | פתרון |
   158||------|--------|--------|
   159|| תיאור מחדש של הסצנה | קליפ חדש, לא המשך | תאר רק מה הלאה |
   160|| שינוי Camera position בלי continuity | קפיצה ויזואלית | camera handoff מדויק |
   161|| שינוי Visual Style | drift, inconsistency | העתק בדיוק |
   162|| בלי Finish Lock | AI מוסיף glow/heroic | תמיד הכנס Finish block |
   163|| פרומפט קצר | חסר כיוון | 5 בלוקים × 3 שניות |
   164|
   165|---
   166|
   167|## תרחישים אמיתיים
   168|
   169|**Action Sequence (Golden Angel style):**
   170|```
   171|קליפ 1: טרנספורמציה — transformation sequence
   172|קליפ 2: Combat pressure — ישות ראשונה
   173|קליפ 3: Combat escalation — ריבוי אויבים
   174|```
   175|
   176|**Brand Film דקה:**
   177|```
   178|קליפ 1: דמות מהלכת ברחוב
   179|קליפ 2: נכנסת לחנות, מגלה מוצר
   180|קליפ 3: רגע רגשי + סגירה
   181|```
   182|
   183|**טבע קולנועי:**
   184|```
   185|קליפ 1: Drone shot יורד מהשמים
   186|קליפ 2: חודר ליער, עוקב אחרי נהר
   187|קליפ 3: מגיע לאגם, שקיעה
   188|```
   189|
   190|---
   191|
   192|## העקרון הגדול
   193|
   194|Seedance מנתח **את כל המסלול** — תנועה, תאורה, קומפוזיציה — לא רק הפריים האחרון.
   195|
   196|תכנון מראש של camera handoff + Visual Style Lock + Finish Block =
   197|סרטון שנראה כמו single continuous take ארוך, ולא כמו קליפים מודבקים יחד.
   198|
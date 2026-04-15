     1|---
     2|name: golden-angel-template
     3|description: >
     4|  תבנית Golden Angel — השיטה המתקדמת ביותר לבניית פרומפטים סינמטיים ב-Seedance 2.0.
     5|  הפעל כאשר המשתמש רוצה: סדרת קליפים רציפה, אקשן סינמטי, טרנספורמציה,
     6|  קרב, fantasy/tokusatsu, או כל סצנה עם דמות ועולם ויזואלי עקבי.
     7|  גם trigger על: "תבנית Golden Angel", "שיטת Golden Angel", "תבנית לסדרה",
     8|  "תכנן לי כמה קליפים", "סדרת וידאו", "כל הפרומפטים לסדרה".
     9|---
    10|
    11|# Golden Angel Template — תבנית מלאה לסדרת קליפים
    12|
    13|## מה זה
    14|
    15|שיטת בניית פרומפטים שפוצחה עבור פרויקט "The Golden Angel" —
    16|שלושה קליפים רצופים שנראים כמו single take קולנועי אחד.
    17|
    18|**שלושת העקרונות הגדולים:**
    19|1. Visual Style Lock — אותו spec ב-100% בכל קליפ
    20|2. Camera Handoff — end position של קליפ N = start position של קליפ N+1
    21|3. Anti-Heroic Constraint — כל עוצמה מלווה בכאב, לא בניצחון
    22|
    23|---
    24|
    25|## שלב 0 — Planning (לפני שכותבים כלום)
    26|
    27|מלא את הטבלה הזו לפני שמתחיל:
    28|
    29|```
    30|שם הפרויקט / האסתטיקה: _______________
    31|ז'אנר: _______________
    32|Visual Style (נעל עכשיו — לא לשנות):
    33|  מפרט: _______________
    34|  פלטה: _______________
    35|  grain: _______________
    36|מילת הטון: _______________ (heavy / painful / cold / raw / dark)
    37|מה לא: _______________ (no glow / no heroic / no beauty)
    38|
    39|Camera Handoff Plan:
    40|  קליפ 1: Start [___] → End [___]
    41|  קליפ 2: Start [___] → End [___]
    42|  קליפ 3: Start [___] → End [___]
    43|
    44|הנרטיב הכולל (3 מצבים):
    45|  קליפ 1: [מצב נרטיבי — transformation / awakening / revelation]
    46|  קליפ 2: [מצב נרטיבי — first pressure / encounter / confrontation]
    47|  קליפ 3: [מצב נרטיבי — escalation / crisis / forced action]
    48|```
    49|
    50|---
    51|
    52|## תבנית קליפ 1 — הטרנספורמציה / פתיחה
    53|
    54|```
    55|Core Theme: [ז'אנר], [אסתטיקה], [מצב נרטיבי — transformation/awakening], [סביבה]
    56|
    57|Character Setup
    58|Face: Use reference@Image1 exactly, [מה לשמר]. No beautification. [expression]:
    59|  [תיאור הבעה] — [מה כן], no [מה לא].
    60|Clothing: [מצב בגד התחלתי — שלם, קודם טרנספורמציה] [נשק אם יש]
    61|Environment: [מה בסצנה]
    62|
    63|Visual Style
    64|[מפרט מצלמה — זהה בכל קליפ]
    65|[פלטה], compressed shadows with texture, slight edge softness, moderate film grain
    66|[שם האסתטיקה]: [תפיסה ויזואלית]
    67|
    68|Camera Rules
    69|Single continuous take
    70|Start [low/high]-angle [right/left] side, [תנועה — orbit/push/drift], end [angle + side]
    71|Subtle handheld "breathing" motion throughout
    72|
    73|0–3s
    74|Camera: [position initial + behavior]
    75|Action: [micro action — subtle, slow]
    76|Environment: [תגובת סביבה לנוכחות הדמות]
    77|
    78|3–6s
    79|Camera: [המשך]
    80|Action: [beat ראשון של שינוי]
    81|Effect: [תגובה פיזית — ללא גלו]
    82|
    83|6–9s
    84|Camera: [תנועה דרמטית — shakes / loses focus]
    85|Action: [beat מרכזי — השינוי הגדול]
    86|Effect: [תוצאה ויזואלית]
    87|
    88|9–12s
    89|Camera: [close-up / emphasis]
    90|Action: [פרט — שיער / עיניים / גוף]
    91|Detail: [תיאור ספציפי]
    92|
    93|12–15s
    94|Camera: [finishes orbit to [end-position]]
    95|Action: [סגירה — פריט מופיע / עמידה חדשה]
    96|Effect: [תגובה פיזית אחרונה]
    97|
    98|Finish: [מפרט טכני], [grade], [fps], sharp, no glow, [מילת הטון] tone
    99|```
   100|
   101|---
   102|
   103|## תבנית קליפ 2 — לחץ ראשון / עימות
   104|
   105|```
   106|Continue the story and scene showing in @video, and maintain all aspects of continuity,
   107|following this prompt:
   108|
   109|Core Theme: [ז'אנר], [אסתטיקה], [מצב נרטיבי — post-[X] / first pressure], [סביבה]
   110|
   111|Character Setup
   112|Face: Use reference@Image1 exactly, [שינוי מינימלי מקליפ 1], no beautification.
   113|  Expression: [רגש עדכני], no heroic energy or eye highlights.
   114|Clothing: [עדכון — חלקית הרוס / עם שינוי מהטרנספורמציה] [נשק נוכחי]
   115|Environment: [עדכון — סביבה מגיבה לטרנספורמציה]
   116|
   117|Visual Style
   118|[העתק מדויק מקליפ 1 — אותן מילים]
   119|
   120|Camera Rules
   121|Single continuous take
   122|Start [end position של קליפ 1], [המשך תנועה], [drift/continuation]
   123|Subtle handheld "breathing" motion throughout
   124|
   125|00–03 Seconds
   126|Camera: [continues from [end position], behavior]
   127|Action: [דמות סטטית — תנועה קטנה בלבד]
   128|Environment: [סביבה מגיבה — ground compresses / ash lifts / energy field]
   129|
   130|03–06 Seconds
   131|Camera: [המשך מסלול]
   132|Action: [ישות/אויב/איום מתגלה בעומק — לא ברור, לא שלם]
   133|Character: [תגובה מינימלית — head shift בלבד]
   134|
   135|06–09 Seconds
   136|Camera: [slight forward push, single take]
   137|Action: [איום לומד לפריים — תנועה פתאומית]
   138|Character: [תגובה מינימלית — limb/wing blocks]
   139|Effect: [shock wave / ground fracture / circular pattern]
   140|
   141|09–12 Seconds
   142|Camera: [loses focus briefly due to impact → regains]
   143|Action: [physical pressure — resistance, not power]
   144|Detail: [skin/armor under tension / hand tightens]
   145|
   146|12–15 Seconds
   147|Camera: [stabilizes slightly, still breathing]
   148|Action: [פעולה אחת — sword/strike/push — short, direct, no flourish]
   149|Effect: [תוצאה מאוחרת — delayed split / fracture / fragments]
   150|
   151|End State (IMPORTANT): [איום לא מת — collapsing but unstable]
   152|[דמות — grounded, not dominant, partial extension/reach, no heroic pose]
   153|
   154|Finish (Consistency Lock): Same [מפרט], Same [grade], [grain]
   155|No added [what not], Everything remains [מילת הטון], painful, physical
   156|```
   157|
   158|---
   159|
   160|## תבנית קליפ 3 — הסלמה / משבר
   161|
   162|```
   163|Continue the story and scene showing in @video, and maintain all aspects of continuity,
   164|following this prompt:
   165|
   166|Core Theme: [ז'אנר], [אסתטיקה], [מצב נרטיבי — full-form under escalating pressure], [סביבה]
   167|
   168|Character Setup
   169|Face: Use reference@Image1 exactly, [שינוי נוסף — יותר מכוסה / פגוע],
   170|  no beautification. Expression: [רגש — heavy / controlled / restrained], no heroic energy.
   171|Clothing: [עדכון — יותר הרוס / שריון מלא / transformation complete] [נשק]
   172|Environment: [עדכון — איום הראשון עדיין נוכח + אויבים חדשים מגיחים]
   173|
   174|Visual Style
   175|[העתק מדויק — זהה ל-100%]
   176|
   177|Camera Rules
   178|Single continuous take
   179|Continue from [end position של קליפ 2] into [unstable orbit / vertical tracking]
   180|Subtle handheld "breathing" motion throughout
   181|
   182|00–03s
   183|Camera: [handheld, slightly tilted, continuing orbit]
   184|Action: [multiple threats emerge from [direction]]
   185|Environment: [ground fractures / ash density / visibility drops]
   186|Character: [remains still at center]
   187|
   188|03–06s
   189|Action: [forced movement — not graceful, yanked/pulled by force]
   190|Camera: [struggles to follow, tilting late]
   191|Environment: [debris/dust drags with movement]
   192|
   193|06–09s
   194|Action: [mid-air threat — minimal rotation, one cut/strike]
   195|Effect: [delayed split / fragments hang before falling]
   196|Action 2: [secondary impact from behind — wing/limb absorbs]
   197|Effect 2: [shock ripples through body]
   198|
   199|09–12s
   200|Camera: [slightly below, unstable framing]
   201|Action: [force compression — air/ground pushed outward]
   202|Effect: [multiple enemies displaced — some hit ground, some suspended]
   203|
   204|12–15s
   205|Action: [sudden drop — fast, uncontrolled]
   206|Camera: [whips down to follow]
   207|Action: [impact — weapon drives into ground]
   208|Effect: [localized shockwave / radial cracks / enemies thrown outward]
   209|
   210|End State
   211|[landing stance — crouched, wings partially open]
   212|[enemies still remain — scattered, not defeated]
   213|[airborne-capable but still heavy, still physical]
   214|
   215|Finish
   216|Same [מפרט], [grade], [grain]
   217|No glow, no fantasy softness
   218|[Movement/power type] feels forced, heavy, and violent — not heroic
   219|```
   220|
   221|---
   222|
   223|## רשימת בדיקה לפני הגנרציה
   224|
   225|לפני שלוחצים Generate על כל קליפ, בדוק:
   226|
   227|קליפ 1:
   228|☐ Visual Style Lock כתוב?
   229|☐ Camera end position מוגדר?
   230|☐ 5 בלוקים × 3 שניות?
   231|☐ End State כתוב?
   232|☐ Finish Lock עם רשימת NOT?
   233|
   234|קליפ 2:
   235|☐ שורת continuity ב-@video?
   236|☐ Camera start = end של קליפ 1?
   237|☐ Visual Style — העתק מדויק?
   238|☐ End State — לא ניצחון?
   239|☐ Finish Lock — זהה?
   240|
   241|קליפ 3:
   242|☐ שורת continuity ב-@video?
   243|☐ Camera start = end של קליפ 2?
   244|☐ Visual Style — העתק מדויק?
   245|☐ Multiple threats?
   246|☐ Forced movement — not graceful?
   247|☐ End State — enemies scattered, not defeated?
   248|☐ Finish Lock — זהה?
   249|
   250|---
   251|
   252|## Anti-Heroic Quick Reference
   253|
   254|כל פעם שאתה כותב פעולה חזקה, הוסף את הכאב:
   255|
   256|| פעולה | הוסף |
   257||-------|-------|
   258|| flies | "yanked upward abruptly, not graceful" |
   259|| blocks | "shock travels through [limb] → into ground" |
   260|| strikes | "short, direct motion, no flourish" |
   261|| power | "no glow increase — air compresses violently" |
   262|| lands | "drops suddenly — fast, uncontrolled descent" |
   263|| wins | "enemies still remain — scattered" |
   264|| stands | "still grounded, still heavy, still physical" |
   265|| moves | "forced, heavy, violent — not heroic" |
   266|
# JRS Metabolism

يتوافق مع jrs_core وjrs_inventory وoxmysql. شغّل هذه الموارد قبل jrs_metabolism.
يحفظ الجوع والعطش لكل شخصية عند الخروج، وتبديل الشخصية، وبشكل دوري. ينشئ جدول الحالة إذا لم يكن موجودًا ويحافظ على السجلات القديمة.
عند أول تشغيل يحوّل أعمدة النسب القديمة من الأعداد الصحيحة إلى أعداد عشرية لحفظ النقص التدريجي بدقة، دون حذف السجلات.
تُعرض صحة اللاعب وتحمّله من اللعبة دون إعادة تطبيق حالة قديمة فوق حالة الكور.
تُستخدم الأطعمة والمشروبات من الإنفنتوري أو عجلة العناصر، وتُحذف قطعة من السلوت المستخدم قبل تطبيق الفائدة.
إعدادات النقص والضرر ومكان المؤشرات في config.lua، وفوائد الأطعمة والمشروبات في consumables.lua.
/hud1 و/hud2 و/hud3 تغيّر مكان المؤشرات. تدعم المؤشرات لغة الشخصية العربية والإنجليزية.

Server exports: varyHunger(source, amount), varyThirst(source, amount), GetStatus(source), RestoreNeeds(source).
Hunger and thirst use deficit values: 0 is full and 100 is empty; a negative variation restores the need.


---

## Part of JRS Core

This resource is part of **[JRS Core](https://github.com/JRS-CORE/jrscore)**, a free, open-source RedM roleplay framework (70+ resources, one txAdmin recipe, English and Arabic).

- Docs: https://docs.jrs-core.com
- Discord: https://discord.gg/jrscore
- License: GNU GPL v3

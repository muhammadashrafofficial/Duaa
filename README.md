<div dir="ltr">

# Duaa · دعاء

**A spiritual companion for Quran, adhkar, and duaa — with Duro the bird by your side.**
**رفيقك الروحاني للقرآن والأذكار والدعاء، ومعك دورو في كل خطوة.**

Duaa is an open-source Android app built entirely with Kotlin and Jetpack Compose. It brings together mushaf reading, audio recitation, daily adhkar, smart duaa suggestions, and personal worship tracking in one dark, royal-themed experience guided by its mascot, Duro.

[![Kotlin](https://img.shields.io/badge/Kotlin-2.x-7F52FF?logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-Material%203-4285F4?logo=jetpackcompose&logoColor=white)](https://developer.android.com/compose)
[![minSdk](https://img.shields.io/badge/minSdk-24-brightgreen)](https://developer.android.com)
[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white)](https://www.android.com)

---

</div>

<div dir="rtl">

## لماذا دعاء؟

في وسط زحمة اليوم، «دعاء» بيجمعلك كل اللي محتاجه لروحك في مكان واحد: تقرأ القرآن، تسمع التلاوة، تقول أذكارك، وتكتب دعواتك. وكل ده ومعاك «دورو»، الطائر الصغير اللي بيقترح عليك الدعاء المناسب للحظة اللي انت فيها.

## المميزات

- **المصحف الكامل**: قراءة بصور الصفحات الأصلية، مع تفسير وحفظ علامات للصفحات.
- **الاستماع للتلاوات**: مجموعة من أشهر القراء، مع تشغيل في الخلفية حتى والشاشة مقفلة.
- **رادار دورو**: اقتراحات دعاء ذكية حسب الوقت والمكان والطقس. مسافر؟ زعلان؟ شاكر؟ دورو يعرف.
- **أذكار الصباح والمساء**: الأذكار كاملة مع عداد التكرار.
- **آية اليوم**: تذكير يومي بآية تبدأ بيها يومك.
- **إحصائيات الاستماع**: تتبع أسبوعي، وسلسلة أيام متواصلة (Streak) تشجعك تكمل.
- **متتبع الختمة**: سجل تقدمك في القراءة ناحية الختمة.
- **يوميات الدعاء**: دفترك الخاص، اكتب دعواتك وارجعلها.
- **ثيم ملكي غامق**: ألوان مستوحاة من دورو نفسه، برتقاني دافي وتركواز على خلفية بنفسجية عميقة.

## لقطات الشاشة
<img width="1080" height="1350" alt="photo_2026-11-26_10-53-04" src="https://github.com/user-attachments/assets/ff34f069-8b16-4429-99a0-dcb58de1e3d9" />


<img width="1080" height="1350" alt="photo_2026-11-26_10-53-03" src="https://github.com/user-attachments/assets/ace1e98b-0b44-4edd-81eb-6fe651a8329a" />


<img width="1080" height="1350" alt="photo_2026-11-26_10-53-01" src="https://github.com/user-attachments/assets/4d968686-74ab-4945-a360-2c76111f0887" />


<img width="1080" height="1350" alt="photo_2026-11-26_10-52-59" src="https://github.com/user-attachments/assets/bdb87965-5f13-4fc7-a406-94295c4b38dd" />


## التحميل

آخر نسخة APK جاهزة على صفحة [Releases](../../releases). حمّل الملف وثبّته على جهازك مباشرة.

</div>

<div dir="ltr">

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Kotlin |
| UI | Jetpack Compose + Material 3 |
| Architecture | MVVM, feature modules |
| DI | Koin |
| Local storage | Room |
| Networking | Retrofit + OkHttp + kotlinx.serialization |
| Audio | Media3 / ExoPlayer (background service) |
| Background work | WorkManager |
| Min / Target SDK | 24 / 37 |

## Architecture

The app follows **MVVM** with a modular-by-feature structure:

- `ui/` — Compose screens and shared theme (Duro palette)
- `data/` — Room database, repositories, Retrofit services
- `player/` — Media3 playback service
- `worker/` — WorkManager jobs (daily ayah, reminders)

Data sources:

- [api.alquran.cloud](https://alquran.cloud/api) — Quran text and tafsir
- [android.quran.com](https://android.quran.com) — mushaf page images
- [rn0x/Adhkar-json](https://github.com/rn0x/Adhkar-json) — morning/evening adhkar

## Build from source


</div>

<div dir="rtl">

## خطة الإصدار الثاني (v2)

- دورو كرفيق تفاعلي داخل التطبيق: يحتفل بسلسلتك ويقترح دعاء اللحظة.
- وضع الحفظ والتسميع: إخفاء جزء من الآية، تكرار مقطع، وتسجيل صوتك ومقارنته بالتلاوة.
- خطة ختمة ذكية بورد يومي حسب المدة اللي تحددها.
- مواقيت الصلاة والتنبيه بالأذان.
- ويدجت للشاشة الرئيسية: آية اليوم والسلسلة.
- تقرير أسبوعي بإنجازاتك.

## المساهمة

أي اقتراح أو تحسين مرحب بيه. افتح Issue أو Pull Request.

## الترخيص

لم يحدد بعد. راجع ملف LICENSE عند إضافته.

</div>

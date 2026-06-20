# ⚡ PowerMusic — مشغل موسيقى مجاني

مشغل موسيقى مشابه لـ Poweramp، مجاني 100% بدون إعلانات.

---

## 🎵 المميزات
- ✅ تشغيل جميع ملفات MP3 / FLAC / WAV / OGG
- ✅ مكتبة أغاني تلقائية من الجهاز
- ✅ بحث في الأغاني
- ✅ إيكوالايزر 5 باندات حقيقي
- ✅ تشغيل في الخلفية مع إشعار تحكم
- ✅ Shuffle و Repeat
- ✅ سيك بار للتقديم والتأخير
- ✅ ديزاين داكن بحال Poweramp

---

## 🚀 طريقة فتح المشروع وبناء APK

### الخطوة 1 — تحميل Android Studio
اذهب لـ: https://developer.android.com/studio
حمّل وثبّت Android Studio.

### الخطوة 2 — فتح المشروع
1. افتح Android Studio
2. اختر **Open**
3. حدد فولدر **PowerMusic**
4. انتظر حتى يحمّل Gradle (دقيقتين تقريباً)

### الخطوة 3 — بناء APK
1. من القائمة العلوية: **Build → Build Bundle(s)/APK(s) → Build APK(s)**
2. انتظر حتى يكتمل البناء
3. اضغط على **locate** في الإشعار السفلي
4. ستجد الـ APK في: `app/build/outputs/apk/debug/app-debug.apk`

### الخطوة 4 — تثبيت على الهاتف
1. انقل ملف الـ APK للهاتف
2. فعّل "تثبيت من مصادر غير معروفة" في الإعدادات
3. افتح الـ APK وثبّته

---

## 📂 هيكل المشروع

```
PowerMusic/
├── app/src/main/
│   ├── java/com/powermusic/app/
│   │   ├── MainActivity.kt      ← شاشة المكتبة
│   │   ├── PlayerActivity.kt    ← شاشة التشغيل + EQ
│   │   ├── MusicService.kt      ← خدمة التشغيل في الخلفية
│   │   ├── SongAdapter.kt       ← قائمة الأغاني
│   │   └── Song.kt              ← موديل الأغنية
│   ├── res/
│   │   ├── layout/              ← واجهات XML
│   │   ├── values/              ← ألوان + نصوص + ثيم
│   │   └── drawable/            ← أيقونات
│   └── AndroidManifest.xml
├── build.gradle
├── settings.gradle
└── gradle.properties
```

---

## 🎨 تخصيص اللون
لتغيير لون accent (الأزرق) غيّر في `res/values/colors.xml`:
```xml
<color name="accent">#5B6EFF</color>  <!-- غيّر هذا -->
```

---

## 📱 المتطلبات
- Android 5.0 (API 21) أو أحدث
- إذن الوصول لملفات الموسيقى

---

صُنع بـ ❤️ — مجاني 100%

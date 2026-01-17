# IQLID Systems Website

موقع شركة إقليد للأنظمة - سيادة التقنية.. ذكاء البناء

## نشر الموقع على GitHub Pages

### الخطوات:

1. **إنشاء مستودع جديد على GitHub:**
   - اذهب إلى github.com وسجل الدخول
   - انقر على "New repository"
   - سمّ المستودع: `iqlid-website` أو `username.github.io`
   - اجعله Public
   - لا تضف README (لدينا واحد)

2. **رفع الملفات:**
   ```bash
   cd C:/Users/mo/iqlid-website
   git init
   git add .
   git commit -m "Initial commit - IQLID Systems website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/iqlid-website.git
   git push -u origin main
   ```

3. **تفعيل GitHub Pages:**
   - اذهب إلى Settings في المستودع
   - انقر على "Pages" من القائمة الجانبية
   - تحت "Source" اختر "Deploy from a branch"
   - اختر "main" branch و "/ (root)"
   - انقر Save

4. **الوصول للموقع:**
   - الموقع سيكون متاحاً على: `https://YOUR_USERNAME.github.io/iqlid-website/`

## ربط الدومين المخصص

لربط الدومين الخاص بك (مثل iqlid.com):

1. في إعدادات GitHub Pages، أضف الدومين في خانة "Custom domain"
2. في لوحة تحكم DNS (Hostinger)، غيّر الـ CNAME record:
   - Type: CNAME
   - Name: www
   - Content: YOUR_USERNAME.github.io
3. للـ root domain، أضف A records تشير إلى:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153

## هيكل الملفات

```
iqlid-website/
├── index.html          # الصفحة الرئيسية
├── css/
│   └── style.css       # ملف التنسيقات
├── js/
│   └── main.js         # ملف JavaScript
├── images/
│   └── logo.png        # شعار الشركة
└── README.md           # هذا الملف
```

## ملاحظات

- أضف صور الشركاء (NVIDIA, Dell, Cisco, Microsoft) في مجلد images
- حدّث معلومات التواصل (الهاتف، البريد) في index.html
- يمكنك إضافة صور لقصص النجاح في مجلد images

---
name: dars-tayyorlash
description: >-
  Web dasturlash kursi roadmapi asosida berilgan dars uchun kunlik dars rejasi,
  interaktiv HTML slayd, amaliy mini-dastur, Git commit va hisobot tayyorlaydi.
  Foydalanuvchi biror dars raqami yoki mavzusini tayyorlashni so'raganda ishlatiladi.
---

# Dars Tayyorlash Jarayoni

Foydalanuvchi biror darsni (masalan, "5-darsni tayyorla" yoki "Flexbox darsini tayyorla") so'raganda quyidagi bosqichlarni ketma-ket bajar:

## 1-bosqich: Roadmapdan mavzuni aniqlash
1. [Web dasturlash kursi — Roadmap (12 yoshli o'quvchilar uchun).md](../../../Web%20dasturlash%20kursi%20—%20Roadmap%20(12%20yoshli%20o'quvchilar%20uchun).md) faylidan kerakli modul va dars qatorini top.
2. Dars raqami (`YYY`), modul raqami (`XX`), nazariya (N), amaliyot (A) va mini-loyiha talablarini ajratib ol.
3. *(Ixtiyoriy)* Agar NotebookLM MCP ulangan bo'lsa, mavzu bo'yicha qiziqarli misollar yoki tushuntirish g'oyalarini qidir.

## 2-bosqich: Kunlik dars rejalari (Asosiy + Mustahkamlash)
1. `darslar/modul-XX/dars-YYY/` papkasini yarat.
2. [dars-rejasi-shablon.md](./resources/dars-rejasi-shablon.md) asosida `dars-rejasi.md` (1-kun: asosiy dars, 45 daqiqa) faylini yoz:
   - `0–5 daqiqa`: Qizdirish (o'tgan darsdan 2–3 savol)
   - `5–15 daqiqa`: Nazariya (maksimum 10 daqiqa, hayotiy o'xshatish bilan)
   - `15–37 daqiqa`: Amaliyot ("Men yozaman — biz yozamiz — sen yozasan")
   - `37–42 daqiqa`: Mini-ish / "Xatoni top" o'yini
   - `42–45 daqiqa`: Yakun (3 ta asosiy fikr + ixtiyoriy uy vazifasi)
3. [amaliy-dars-rejasi-shablon.md](./resources/amaliy-dars-rejasi-shablon.md) asosida `amaliy-dars-rejasi.md` (2-kun: **45 daqiqalik to'liq amaliy mustahkamlash darsi**) faylini yoz:
   - Yangi nazariya bo'lmasin; butun 45 daqiqa oldingi darsni mustahkamlashga qaratilsin (`0–5` tezkor takrorlash, `5–35` 3 darajali amaliy topshiriqlar: Oson → O'rta → Yulduzcha, `35–42` "Xato ovchisi" / juftlik tekshiruvi, `42–45` baholash).

## 3-bosqich: Interaktiv HTML slayd yaratish
1. [slayd-shablon.html](./resources/slayd-shablon.html) andozasidan foydalanib, tashqi kutubxonalarsiz (offline ham ishlaydigan) `darslar/modul-XX/dars-YYY/slayd.html` faylini yarat.
2. Slayd tarkibi:
   - 1-slayd: Mavzu nomi va modul
   - 2-slayd: Qizdirish savollari
   - 3–5-slaydlar: Nazariya (katta shrift, o'xshatish, qisqa matn, rangli kod namunalari)
   - 6-slayd: Amaliy topshiriq va "Xatoni top" mashqi
   - 7-slayd: Yakun (3 ta asosiy xulosa va keyingi darsga qiziqtirish)
3. Klaviatura (`←` / `→` / `Space`) va tugmalar bilan boshqarish ishlashini ta'minla.

## 4-bosqich: Amaliy mini-dastur va topshiriqlar tayyorlash
1. `darslar/modul-XX/dars-YYY/amaliyot/` papkasida quyidagi 3 ta faylni yarat:
   - `index.html` — brauzerda darhol ishlaydigan tayyor namuna ("Men yozaman" bosqichi uchun, o'zbekcha izohlar bilan).
   - `starter.html` — **keyingi 45 daqiqalik mustahkamlash darsi** uchun o'quvchilar to'ldirib bajaradigan boshlang'ich shablon (`<!-- TOPSHIRIQ 1 -->`, `<!-- TOPSHIRIQ 2 -->`, `<!-- YULDUZCHA TOPSHIRIQ -->` izohlari bilan).
   - `xatoni-top.html` — 3 ta ataylab qilingan xatoli "Xato ovchisi" mashqi.

## 5-bosqich: Git'ga yuklash va hisobot tayyorlash
1. `git status` va `git add darslar/modul-XX/dars-YYY/` orqali fayllarni qo'shib, `git commit -m "dars-YYY: <mavzu>"` bajar.
2. `git remote -v` ni tekshir: agar `origin` mavjud bo'lsa `git push` qil; bo'lmasa lokal commit hash (`git rev-parse --short HEAD`) ni ol.
3. [hisobot-shablon.md](./resources/hisobot-shablon.md) asosida `darslar/modul-XX/dars-YYY/hisobot.md` faylini yarat (agar hisobot commitdan keyin yaratilsa, `hisobot.md` ni ham qo'shib `--amend` yoki alohida commit qil).
4. Foydalanuvchiga kunlik dars rejasi xulosasini, yaratilgan fayllar havolalarini va slayd/amaliyotni ochish ko'rsatmasini taqdim et.

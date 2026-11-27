# Dars №010: Audio va video (`<audio>`, `<video>`)

- **Modul:** 01-modul — HTML asoslari (1–18-darslar)
- **Davomiyligi:** 45 daqiqa
- **Maqsad:** Veb-sahifaga `<audio>` va `<video>` teglari yordamida ovoz hamda video joylashtirishni, `controls`, `loop`, `muted`, `poster` atributlaridan to'g'ri foydalanishni o'rganish.
- **Kerakli vositalar:** VS Code, Live Server, Google Chrome, [slayd.html](./slayd.html), [amaliyot/index.html](./amaliyot/index.html), [amaliyot/xatoni-top.html](./amaliyot/xatoni-top.html)

---

## 45 daqiqalik dars rejasi

### 1. Qizdirish (0–5 daqiqa)
O'tgan 9-dars ("Jadvallar") bo'yicha 3 ta tezkor savol:
1. HTML da jadval ochish uchun qaysi teg ishlatiladi? (`<table>`)
2. Jadvalning bitta qatorini yaratish uchun-chi? (`<tr>`)
3. Sarlavha katakchasi (`<th>`) oddiy katakchadan (`<td>`) nimasi bilan farq qiladi? (Qalin va markazda chiqadi)

### 2. Nazariya (5–15 daqiqa — maksimum 10 daqiqa)
- **Hayotiy o'xshatish:**
  - `<audio>` — bu cho'ntagingizdagi **musiqa pleyeri**.
  - `<video>` — bu sahifadagi **kichik televizor (yoki YouTube oynasi)**.
  - `controls` atributi — bu **pult va tugmalar** (Play, Pause, ovoz balandligi). Agar `controls` yozilmasa, pleyer ko'rinmaydi — xuddi tugmalarsiz televizordek!
- **Asosiy teglar va atributlar:**
  - `<audio controls>` va ichida `<source src="musiqa.mp3" type="audio/mpeg">`
  - `<video controls width="400" poster="muqova.jpg">` va ichida `<source src="video.mp4" type="video/mp4">`
  - Qo'shimcha atributlar: `loop` (qayta-qayta ijro), `muted` (ovozsiz boshlash), `autoplay` (avto-ijro — odatda `muted` bilan ishlaydi).
- **Xavfsizlik va mualliflik huquqi:** Boshqa saytlardan musiqa yoki video olayotganda ruxsat etilgan (bepul/ochiq litsenziyali) fayllardan foydalanish kerak.
- **Jonli namoyish:** O'qituvchi ekranda `<audio controls>` kodini yozib, brauzerda pleyer paydo bo'lishini ko'rsatadi.

### 3. Amaliyot (15–37 daqiqa — 22 daqiqa)
- **"Men yozaman" (5 daqiqa):** O'qituvchi [amaliyot/index.html](./amaliyot/index.html) faylini Live Server'da ochib, sahifada audio pleyer va video oynasi qanday ishlashini ko'rsatadi.
- **"Biz yozamiz" (7 daqiqa):** O'quvchilar bilan birgalikda pleyerga `loop` atributi qo'shiladi, video kengligi (`width`) o'zgartiriladi va `<audio>` ostiga qo'shiq nomi yoziladi.
- **"Sen yozasan" (10 daqiqa):** Har bir o'quvchi o'z sahifasiga:
  1. Sevimli qo'shig'i yoki ovoz effekti uchun `<audio controls>` qo'shadi.
  2. Video bloki uchun `<video controls width="360">` yozadi va unga qisqa tavsif (`<p>`) qo'shadi.
  *(Juftlikda ishlash: "haydovchi" kod yozadi, "navigator" teglarning yopilishini tekshiradi; 5 daqiqadan so'ng rollar almashadi.)*

### 4. Mini-ish / "Xatoni top" o'yini (37–42 daqiqa)
- O'quvchilar [amaliyot/xatoni-top.html](./amaliyot/xatoni-top.html) faylidagi **3 ta ataylab qilingan xatoni** topishadi:
  1. `controls` atributi tushib qolgan (`<audio>` ko'rinmayapti).
  2. `<source>` ichida `src` o'rniga `scr` deb xato yozilgan.
  3. `<video>` tegi yopilmagan (`</video>` yo'q).
- Birinchi bo'lib 3 ta xatoni tuzatgan o'quvchiga **"Xato ovchisi"** nishoni (yulduzcha) beriladi.

### 5. Yakun (42–45 daqiqa)
- **3 ta asosiy fikr:**
  1. Ovoz uchun `<audio>`, video uchun `<video>` tegi ishlatiladi.
  2. Boshqaruv tugmalari ko'rinishi uchun albatta `controls` yozish shart.
  3. Fayl manzili `<source src="..." type="...">` ichida ko'rsatiladi.
- **Ixtiyoriy uyga vazifa:** O'zingizning "Men haqimda" sahifangizga sevimli tabiat ovozi yoki qisqa video bloki qo'shib keling.
- **Keyingi darsda (11-dars):** Saytga foydalanuvchi o'z ismini va parolini kiritadigan **Formalar** (`<form>`, `<input>`) yasashni o'rganamiz!

<details>
   <summary>CSS stillash (CSS Styling / Стилизация CSS)</summary>


**CSS nima? (What is CSS? / Что такое CSS?)**

CSS (Cascading Style Sheets / Каскадные таблицы стилей) veb-sahifalarni bezash va ularga stil berish uchun ishlatiladigan tildir. CSS yordamida siz matnning rangini, shriftini, o'lchamini, elementlarning joylashuvini, fon rasmlarini va boshqa ko'p narsalarni o'zgartirishingiz mumkin. CSS HTML bilan birgalikda ishlaydi va veb-sahifalaringizni yanada jozibador va foydalanuvchilar uchun qulay qiladi.

**CSS-ni HTML ga ulash (Linking CSS to HTML / Подключение CSS к HTML)**

CSS-ni HTML ga ulashning uchta asosiy usuli mavjud:

1. **Tashqi fayl (External Stylesheet / Внешняя таблица стилей):** Bu eng keng tarqalgan usul. Siz CSS qoidalarini alohida `.css` fayliga yozasiz va uni `<link>` tegi yordamida HTML hujjatiga ulaysiz.

   ```html
   <link rel="stylesheet" href="style.css">
   ```

2. **Ichki stil (Internal Stylesheet / Внутренняя таблица стилей):** Bu usulda CSS qoidalari `<style>` teglari ichida, HTML hujjatining `<head>` qismida yoziladi.

   ```html
   <head>
       <style>
           /* CSS qoidalari bu yerda */
       </style>
   </head>
   ```

3. **Inline stil (Inline Style / Встроенный стиль):** Bu usulda CSS qoidalari to'g'ridan-to'g'ri HTML tegining `style` atributida yoziladi.

   ```html
   <p style="color: blue;">Bu ko'k rangli xatboshi.</p>
   ```

**CSS selektorlari (CSS Selectors / Селекторы CSS)**

CSS selektorlari HTML elementlarini tanlash uchun ishlatiladi. Selektorlar yordamida siz qaysi elementlarga stil berishni aniqlaysiz.

Ba'zi asosiy selektorlar:

* **Teg selektori (Element Selector / Селектор элемента):** Element nomini tanlaydi (masalan, `p`, `h1`, `div`).
* **Klass selektori (Class Selector / Селектор класса):** `class` atributi qiymati bo'yicha elementlarni tanlaydi (masalan, `.highlight`).
* **ID selektori (ID Selector / Селектор ID):** `id` atributi qiymati bo'yicha elementlarni tanlaydi (masalan, `#menu`).

**CSS xossalari va qiymatlari (CSS Properties and Values / Свойства и значения CSS)**

CSS xossalari elementlarning ko'rinishini o'zgartirish uchun ishlatiladi. Har bir xossa o'z qiymatiga ega. Xossalar va qiymatlar CSS qoidalarini tashkil qiladi.

```css
selector {
  xossa: qiymat;
}
```

Masalan, quyidagi qoida barcha `p` teglarining matn rangini ko'k rangga o'zgartiradi:

```css
p {
  color: blue;
}
```

Bu yerda `p` - selektor, `color` - xossa, `blue` esa qiymat.

**Ranglar (Colors / Цвета)**

CSS da ranglarni belgilashning bir necha yo'li mavjud:

* **Rang nomlari (Color names / Названия цветов):** Masalan, `red`, `blue`, `green`, `black`, `white`.
* **Hex kodlar (Hex codes / Hex-коды):** Masalan, `#ff0000` (qizil), `#0000ff` (ko'k), `#008000` (yashil).
* **RGB qiymatlari (RGB values / RGB-значения):** Masalan, `rgb(255, 0, 0)` (qizil), `rgb(0, 0, 255)` (ko'k), `rgb(0, 128, 0)` (yashil).

**Fon (Background / Фон)**

* **`background-color`:** Elementning fon rangini o'rnatadi.

**Chegara (Border / Граница)**

* **`border`:** Element atrofida chegara chizadi. `border` xossasi chegara qalinligini, stilini va rangini bir vaqtning o'zida o'rnatish uchun ishlatilishi mumkin. Masalan, `border: 2px solid red;` 2 piksel qalinlikdagi, to'g'ri chiziqli, qizil rangli chegara chizadi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 1: Tashqi CSS faylini yarating va uni HTML ga ulang.**
    * `style.css` nomli yangi fayl yarating.
    * Ushbu faylga ba'zi CSS qoidalarini yozing. Masalan:
        * `body` tegining fon rangini och yashil rangga (`lightgreen`) o'zgartiring.
        * `h1` tegining matn rangini ko'kga (`blue`) va o'lchamini `36px` ga o'rnating.
        * `p` tegining matn rangini qizilga (`red`) va shriftini `Arial` ga o'zgartiring.
    * HTML faylingizda `<link>` tegini ishlatib, `style.css` faylini ulang.
    * Fayllarni saqlang va brauzerda yangilang. CSS stillari veb-sahifaga qo'llanilganini ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>CSS stillash</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <h1>Bu sarlavha</h1>
        <p>Bu matn.</p>
    </body>
    </html>
    ```

    ```css
    body {
      background-color: lightgreen;
    }
    
    h1 {
      color: blue;
      font-size: 36px;
    }
    
    p {
      color: red;
      font-family: Arial, sans-serif;
    }
    ```

* **Vazifa 2: Ichki stil yordamida elementlarga stil bering.**
    * HTML faylingizning `<head>` qismida `<style>` teglarini yarating.
    * `<style>` teglarining ichida CSS qoidalarini yozing. Masalan:
        * `h2` tegining matn rangini sariqqa (`yellow`) va shrift o'lchamini `24px` ga o'rnating.
        * `a` teglarining rangini yashilga (`green`) va chizilgan chiziqni olib tashlang (`text-decoration: none;`).
    * Faylni saqlang va brauzerda yangilang. CSS stillari veb-sahifaga qo'llanilganini ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>CSS stillash</title>
        <style>
          h2 {
            color: yellow;
            font-size: 24px;
          }
          
          a {
            color: green;
            text-decoration: none;
          }
        </style>
    </head>
    <body>
        <h2>Bu kichik sarlavha</h2>
        <a href="#">Bu havola</a>
    </body>
    </html>
    ```

* **Vazifa 3: Inline stil va chegaralar bilan ishlang.**
    * HTML faylingizda biror elementni tanlang (masalan, bitta `<p>` tegi).
    * Ushbu elementga `style` atributi qo'shing va unga CSS qoidalarini yozing. Masalan, xatboshining rangini to'q ko'k rangga (`#000080`) va shrift o'lchamini `18px` ga o'zgartiring.
    * Xuddi shu elementga `style` atributi orqali qalinligi 5px, stillari `dotted` va rangi `orange` bo'lgan chegara qo'shing.
    * Faylni saqlang va brauzerda yangilang. CSS stili elementga qo'llanilganini ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>CSS stillash</title>
    </head>
    <body>
        <p style="color: #000080; font-size: 18px; border: 5px dotted orange;">Bu xatboshi.</p>
    </body>
    </html>
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  "Mening sevimli taomlarim"**
    * "Mening sevimli taomlarim" (My favorite foods / Мои любимые блюда) deb nomlangan veb-sahifa yarating.
    * Sevimli taomlaringiz ro'yxatini tuzing (kamida 5 ta).
    * Har bir taom uchun alohida bo'lim (`<div>`) yarating.
    * Bo'limlarga sarlavhalar (`<h2>` yoki `<h3>`) qo'shing va taomlarning nomlarini yozing.
    * Har bir bo'limda taom haqida qisqacha ma'lumot bering va rasm qo'shing.
    * CSS yordamida quyidagi stillarni qo'llang:
        * Sahifaning fon rangini o'zgartiring.
        * Sarlavhalar uchun o'zingiz yoqtirgan shriftni, rangni va o'lchamni tanlang.
        * Xatboshilar uchun matn rangini va shrift o'lchamini o'zgartiring.
        * Rasmlarga kenglik va balandlik bering.
        * Har bir bo'limga chegara qo'shing.

    **Kod namunasi:** (bu yerda faqat CSS stillari uchun namuna keltirilgan)

    ```css
    body {
      background-color: #f0f0f5; /* Juda och kulrang fon */
    }
    
    h3 { /* Taom nomlari uchun stil */
      font-family: 'Courier New', monospace;
      color: #8B4513; /* Jigarrang rang */
      font-size: 20px;
      text-align: center;
    }
    
    div { /* Har bir taom uchun stil */
      border: 2px dashed #8B4513;
      margin: 15px;
      padding: 10px;
    }
    ```

* **2-vazifa:  "Sayohatlarim"**
    * "Sayohatlarim" (My travels / Мои путешествия) deb nomlangan veb-sahifa yarating.
    * Sayohat qilgan yoki sayohat qilishni istagan joylaringiz haqida ma'lumot bering.
    * Har bir joy uchun alohida bo'lim (`<div>`) yarating.
    * Bo'limlarga sarlavhalar (`<h2>` yoki `<h3>`) qo'shing va joylarning nomlarini yozing.
    * Har bir bo'limda joy haqida qisqacha ma'lumot bering, rasmlar qo'shing va tegishli veb-saytlarga havolalar bering.
    * CSS yordamida quyidagi stillarni qo'llang:
        * Sahifaning fon rasmini o'rnating.
        * Sarlavhalar uchun o'zingiz yoqtirgan shriftni, rangni va o'lchamni tanlang.
        * Xatboshilar uchun matn rangini va shrift o'lchamini o'zgartiring.
        * Rasmlarga chegara qo'shing va ularning o'lchamlarini moslang.
        * Havolalar uchun rangni va chizilgan chiziqni o'rnating.

    **Kod namunasi:** (bu yerda faqat CSS stillari uchun namuna keltirilgan)

    ```css
    body {
      background-image: url("sayohat.jpg"); /* Fon rasmi */
      background-size: cover; /* Rasmni butun sahifaga yoyish */
    }
    
    h2 {
      font-family: 'Impact', sans-serif;
      color: white;
      text-shadow: 2px 2px 4px black; /* Matnga soya qo'shish */
    }
    
    a {
      color: yellow;
      font-weight: bold;
    }
    ```

* **3-vazifa:  "Mening uy hayvonlarim"**
    * "Mening uy hayvonlarim" (My pets / Мои домашние животные) deb nomlangan veb-sahifa yarating.
    * Uy hayvonlaringiz haqida ma'lumot bering (agar bo'lmasa, o'zingiz yoqtirgan hayvonlar haqida yozing).
    * Har bir hayvon uchun alohida bo'lim (`<div>`) yarating.
    * Bo'limlarga sarlavhalar (`<h2>` yoki `<h3>`) qo'shing va hayvonlarning nomlarini yozing.
    * Har bir bo'limda hayvon haqida qisqacha ma'lumot bering, rasmlar qo'shing.
    * CSS yordamida quyidagi stillarni qo'llang:
        * Sahifaning fon rangini o'zgartiring.
        * Sarlavhalar uchun o'zingiz yoqtirgan shriftni, rangni va o'lchamni tanlang.
        * Xatboshilar uchun matn rangini va shrift o'lchamini o'zgartiring.
        * Rasmlarga chegara qo'shing va ularning o'lchamlarini moslang.

    **Kod namunasi:** (bu yerda faqat CSS stillari uchun namuna keltirilgan)

    ```css
    body {
      background-color: #ffe4c4; /* Bej rang fon */
    }
    
    h3 {
      font-family: 'Lucida Console', monospace;
      color: #800000; /* To'q qizil rang */
      font-size: 22px;
      text-align: right;
    }
    
    img {
      float: right;
      margin-left: 10px;
      border: 4px double #800000;
    }
    ```

</details>

<details>
   <summary>Matn xossalari (Text Properties / Свойства текста)</summary>


**Matn xossalari (Text Properties / Свойства текста)**

CSS da matnning ko'rinishini o'zgartirish uchun turli xil xossalardan foydalanish mumkin. 

* **`color`:** Matn rangini o'rnatadi. Qiymat sifatida rang nomlari, hex kodlar, RGB/RGBA qiymatlari ishlatilishi mumkin.
    * Misol: `color: blue;` (ko'k rang), `color: #ff0000;` (qizil rang), `color: rgb(0, 128, 0);` (yashil rang).
* **`font-family`:** Matn shriftini o'rnatadi. Qiymat sifatida shrift nomlari (masalan, Arial, Times New Roman, Verdana) yoki shrift oilalari (masalan, sans-serif, serif, monospace) ishlatilishi mumkin.
    * Misol: `font-family: Arial, sans-serif;`
* **`font-size`:** Matn o'lchamini o'rnatadi. Qiymat sifatida piksel (`px`), foiz (`%`), em, rem kabi o'lchov birliklari ishlatilishi mumkin.
    * Misol: `font-size: 16px;`, `font-size: 1.2em;`
* **`font-weight`:** Matnning qalinligini o'rnatadi. Qiymat sifatida `normal`, `bold`, `bolder`, `lighter` yoki raqamlar (100 dan 900 gacha) ishlatilishi mumkin.
    * Misol: `font-weight: bold;`
* **`text-align`:** Matnni tekislashni o'rnatadi. Qiymat sifatida `left`, `center`, `right` yoki `justify` ishlatilishi mumkin.
    * Misol: `text-align: center;` (matnni markazga tekislash)
* **`text-decoration`:** Matnga qo'shimcha bezaklar qo'shadi. Qiymat sifatida `none`, `underline`, `overline`, `line-through` ishlatilishi mumkin.
    * Misol: `text-decoration: underline;` (matn ostiga chiziq chizish)
* **`line-height`:** Satrlar orasidagi masofani o'rnatadi. Qiymat sifatida raqamlar yoki o'lchov birliklari ishlatilishi mumkin.
    * Misol: `line-height: 1.5;`

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 4: Matn xossalarini qo'llang.**
    * HTML faylingizda turli xil matn elementlari yarating (masalan, `<h1>`, `<h2>`, `<p>`, `<span>`).
    * CSS faylingizda bu elementlarga turli xil matn xossalarini qo'llang. Masalan, rangini, shriftini, o'lchamini, qalinligini, hizalanishini va bezaklarini o'zgartiring.
    * Faylni saqlang va brauzerda yangilang. O'zgarishlarni kuzating.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>CSS stillash</title>
      <link rel="stylesheet" href="style.css">
    </head>
    <body>
      <h1>Bu sarlavha</h1>
      <h2>Bu kichik sarlavha</h2>
      <p>Bu matn.</p>
      <p>Bu <span>yana bir</span> matn.</p>
    </body>
    </html>
    ```

    ```css
    h1 {
      color: blue;
      font-family: sans-serif;
      font-size: 36px;
      font-weight: bold;
      text-align: center;
      text-decoration: underline;
    }
    
    h2 {
      color: green;
      font-family: serif;
      font-size: 24px;
      font-weight: normal;
      text-align: right;
    }
    
    p {
      color: gray;
      font-family: monospace;
      font-size: 16px;
      font-weight: lighter;
      text-align: justify;
      line-height: 1.5;
    }
    
    span {
      color: red;
      font-weight: bold;
      text-decoration: overline;
    }
    ```

* **Vazifa 5: Shriftlarni import qiling.**
    * Google Fonts yoki boshqa shrift kutubxonasidan shriftni tanlang va uni CSS faylingizga import qiling.
    * Import qilingan shriftni HTML elementlariga qo'llang.

    ```css
    /* Google Fonts dan shriftni import qilish */
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
    
    body {
      font-family: 'Roboto', sans-serif;
    }
    ```

* **Vazifa 6: Matn soyasini qo'shing.**
    * CSS faylingizda `text-shadow` xossasidan foydalanib, matnga soya qo'shing.
    * Soya rangini, x va y o'qlar bo'yicha siljishini va soya radiusini o'zgartirib ko'ring.

    ```css
    h1 {
      text-shadow: 2px 2px 5px gray;
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Turli xil matn stillarini qo'llang**
    * HTML faylingizda turli xil matn elementlari yarating (sarlavhalar, xatboshilar, ro'yxatlar).
    * CSS faylingizda bu elementlarga turli xil matn xossalarini qo'llang.
    * Ranglar, shriftlar, o'lchamlar, qalinlik, hizalanish, bezaklar va qatorlar orasidagi masofa bilan tajriba o'tkazing.

    ```css
    h1 {
      font-family: 'Courier New', Courier, monospace;
      font-size: 48px;
      font-weight: 900;
      color: #A52A2A; /* Jigarrang */
      text-align: center;
    }
    
    h2 {
      font-family: 'Times New Roman', Times, serif;
      font-size: 36px;
      font-weight: normal;
      color: #00008B; /* To'q ko'k */
      text-align: right;
      text-decoration: underline;
    }
    
    p {
      font-family: 'Arial', sans-serif;
      font-size: 16px;
      color: #2F4F4F; /* To'q kulrang-yashil */
      line-height: 1.8;
    }
    ```

* **2-vazifa:  Iqtibosni stillashtiring**
    * HTML faylingizda iqtibos (`<blockquote>`) yarating.
    * CSS faylingizda iqtibosni stillashtiring.
    * Iqtibosning fon rangini, chegara stilini, matn rangini va shriftini o'zgartiring.

    ```css
    blockquote {
      background-color: #f9f9f9;
      border-left: 5px solid #ccc;
      padding: 10px;
      font-style: italic;
      font-size: 18px;
    }
    ```

* **3-vazifa:  Kod bloklarini stillashtiring**
    * HTML faylingizda kod bloklarini (`<code>`) yarating.
    * CSS faylingizda kod bloklarini stillashtiring.
    * Kod bloklarining fon rangini, chegara stilini, matn rangini va shriftini o'zgartiring.

    ```css
    code {
      background-color: #eee;
      border: 1px solid #999;
      padding: 5px;
      font-family: 'Courier New', Courier, monospace;
      font-size: 14px;
    }
    ```
</details>

<details>
   <summary>Fon xossalari (Background Properties / Свойства фона)</summary>


**Fon xossalari (Background Properties / Свойства фона)**

CSS da elementlarning fonini stillashtirish uchun turli xil xossalardan foydalanish mumkin. 

* **`background-color`:** Elementning fon rangini o'rnatadi. Qiymat sifatida rang nomlari, hex kodlar, RGB/RGBA qiymatlari ishlatilishi mumkin.
    * Misol: `background-color: lightblue;` (och ko'k rang), `background-color: #f0f0f0;` (och kulrang rang), `background-color: rgb(255, 255, 0);` (sariq rang).
* **`background-image`:** Elementning fon rasmini o'rnatadi. Qiymat sifatida `url()` funksiyasi yordamida rasm faylining manzilini ko'rsatish kerak.
    * Misol: `background-image: url("fon.jpg");`
* **`background-repeat`:** Fon rasmining takrorlanishini o'rnatadi. Qiymat sifatida `repeat` (standart qiymat, rasm gorizontal va vertikal ravishda takrorlanadi), `repeat-x` (rasm faqat gorizontal ravishda takrorlanadi), `repeat-y` (rasm faqat vertikal ravishda takrorlanadi) yoki `no-repeat` (rasm takrorlanmaydi) ishlatilishi mumkin.
    * Misol: `background-repeat: no-repeat;`
* **`background-position`:** Fon rasmining joylashuvini o'rnatadi. Qiymat sifatida kalit so'zlar (masalan, `top`, `left`, `center`, `bottom`, `right`) yoki foizlar ishlatilishi mumkin.
    * Misol: `background-position: center;` (rasmni markazga joylashtirish)
* **`background-size`:** Fon rasmining o'lchamini o'rnatadi. Qiymat sifatida `cover` (rasm konteynerni to'liq qoplaydi, nisbati saqlanadi), `contain` (rasm konteynerga to'liq sig'adi, nisbati saqlanadi) yoki o'lchov birliklari (masalan, `100px`, `50%`) ishlatilishi mumkin.
    * Misol: `background-size: cover;`

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 7: Fon rangini o'rnating.**
    * HTML faylingizda bir nechta elementlar yarating (masalan, `<h1>`, `<p>`, `<div>`).
    * CSS faylingizda bu elementlarning fon rangini (`background-color`) turli xil ranglarga o'rnating.

    ```css
    body {
      background-color: #f0f0f0; /* Och kulrang */
    }
    
    h1 {
      background-color: lightblue;
    }
    
    p {
      background-color: #e0ffff; /* Och ko'k */
    }
    ```

* **Vazifa 8: Fon rasmini qo'shing.**
    * HTML faylingizda biror element yarating (masalan, `<div>`).
    * CSS faylingizda bu elementga fon rasmini (`background-image`) qo'shing.
    * Rasmning takrorlanishini (`background-repeat`) va joylashuvini (`background-position`) sozlang.

    ```css
    div {
      background-image: url("fon.jpg");
      background-repeat: no-repeat;
      background-position: center;
    }
    ```

* **Vazifa 9: Fon rasmining o'lchamini o'zgartiring.**
    * Yuqoridagi vazifada qo'shgan fon rasmining o'lchamini (`background-size`) `cover` va `contain` qiymatlari bilan o'zgartirib ko'ring.
    * Farqni kuzating.

    ```css
    div {
      background-image: url("fon.jpg");
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover; /* yoki contain */
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Gradient fon yarating.**
    * HTML faylingizda biror element yarating.
    * CSS faylingizda `linear-gradient()` funksiyasidan foydalanib, bu elementga gradient fon yarating.
    * Gradientning ranglarini, yo'nalishini va boshqa xususiyatlarini o'zgartirib ko'ring.

    ```css
    div {
      background: linear-gradient(to right, red, yellow);
    }
    ```

* **2-vazifa:  Fon rasmi bilan matnni stillashtiring.**
    * HTML faylingizda fon rasmi bo'lgan element yarating va uning ichida matn qo'shing.
    * CSS faylingizda matn rangini va soyasini (`text-shadow`) o'rnatib, matnni fon rasmi ustida yaxshi ko'rinishini ta'minlang.

    ```css
    div {
      background-image: url("fon.jpg");
      background-size: cover;
      color: white;
      text-shadow: 2px 2px 4px black;
      padding: 20px;
    }
    ```

* **3-vazifa:  Shaxsiy veb-saytni fon rasmlari bilan bezang.**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini fon rasmlari bilan bezang.
    * Sahifaning umumiy fon rasmini, shuningdek, alohida bo'limlar uchun fon rasmlarini qo'shing.
    * `background-repeat`, `background-position` va `background-size` xossalaridan foydalanib, rasmlarni sozlang.
</details>

<details>
   <summary>Chegara xossalari (Border Properties / Свойства границы)</summary>



**Chegara xossalari (Border Properties / Свойства границы)**

CSS da elementlar atrofida chegara chizish uchun `border` xossasidan foydalaniladi. `border` xossasi quyidagi uchta xususiyatni o'z ichiga oladi:

* **`border-width`:** Chegara qalinligini belgilaydi. Qiymat sifatida piksel (`px`), em, rem kabi o'lchov birliklari ishlatilishi mumkin.
    * Misol: `border-width: 2px;`
* **`border-style`:** Chegara stilini belgilaydi. Qiymat sifatida `solid` (to'g'ri chiziq), `dashed` (punktir chiziq), `dotted` (nuqtali chiziq), `double` (ikki qatorli chiziq), `groove`, `ridge`, `inset`, `outset` (turli xil 3D effektlar) ishlatilishi mumkin.
    * Misol: `border-style: dashed;`
* **`border-color`:** Chegara rangini belgilaydi. Qiymat sifatida rang nomlari, hex kodlar, RGB/RGBA qiymatlari ishlatilishi mumkin.
    * Misol: `border-color: red;`

`border` xossasidan tashqari, har bir xususiyatni alohida-alohida ham o'rnatish mumkin:

```css
border-top-width: 1px;
border-right-style: solid;
border-bottom-color: blue;
```

Bundan tashqari, `border` xossasini qisqa formatda ham yozish mumkin:

```css
border: 2px solid red; /* qalinligi 2px, stili solid, rangi red */
```

**Chegaraning radiusini o'zgartirish (Border Radius / Радиус границы)**

CSS da elementlarning burchaklarini yumaloq qilish uchun `border-radius` xossasidan foydalaniladi. Qiymat sifatida piksel (`px`), foiz (`%`) yoki em kabi o'lchov birliklari ishlatilishi mumkin.

```css
border-radius: 10px; /* barcha burchaklarni 10px ga yumaloq qilish */
```

Burchaklarni alohida-alohida yumaloq qilish uchun quyidagi xossalardan foydalanish mumkin:

* `border-top-left-radius`
* `border-top-right-radius`
* `border-bottom-right-radius`
* `border-bottom-left-radius`

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 10: Elementlarga chegara qo'shing.**
    * HTML faylingizda bir nechta elementlar yarating (masalan, `<h1>`, `<p>`, `<div>`).
    * CSS faylingizda bu elementlarga turli xil chegara stillarini qo'llang.
    * Chegara qalinligini, stilini va rangini o'zgartirib ko'ring.

    ```css
    h1 {
      border: 3px solid blue;
    }
    
    p {
      border-top: 1px dashed red;
      border-bottom: 2px dotted green;
    }
    
    div {
      border-left: 5px double purple;
    }
    ```

* **Vazifa 11: Chegaraning radiusini o'zgartiring.**
    * Yuqoridagi vazifada yaratgan elementlarning burchaklarini yumaloq qiling.
    * `border-radius` xossasidan foydalaning.
    * Turli xil qiymatlar bilan tajriba o'tkazing.

    ```css
    h1 {
      border: 3px solid blue;
      border-radius: 10px;
    }
    ```

* **Vazifa 12: Faqat ba'zi burchaklarni yumaloq qiling.**
    * Yuqoridagi vazifada yaratgan elementlardan birini tanlang.
    * Faqat yuqori chap va pastki o'ng burchaklarni yumaloq qiling.

    ```css
    h1 {
      border: 3px solid blue;
      border-top-left-radius: 20px;
      border-bottom-right-radius: 20px;
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Tugmani stillashtiring.**
    * HTML faylingizda tugma (`<button>`) yarating.
    * CSS faylingizda tugmani stillashtiring.
    * Tugmaga chegara qo'shing, fon rangini o'zgartiring, matn rangini o'zgartiring, burchaklarni yumaloq qiling.

    ```css
    button {
      background-color: #4CAF50; /* Yashil */
      border: none;
      color: white;
      padding: 15px 32px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
      font-size: 16px;
      border-radius: 5px;
    }
    ```

* **2-vazifa:  Kartani stillashtiring.**
    * HTML faylingizda karta (card / карточка) yarating. Kartada rasm, sarlavha va matn bo'lishi mumkin.
    * CSS faylingizda kartani stillashtiring.
    * Kartaga chegara qo'shing, fon rangini o'zgartiring, burchaklarni yumaloq qiling, soyani qo'shing (`box-shadow`).

    ```css
    .card {
      background-color: white;
      border: 1px solid #ccc;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    }
    ```

* **3-vazifa:  Shaxsiy veb-saytni stillashtiring.**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini CSS yordamida yanada stillashtiring.
    * Turli xil chegara stillarini qo'llang.
    * Elementlarning burchaklarini yumaloq qiling.
</details>

<details>
   <summary>Box Model (Box Model / Модель коробки)</summary>


**Box Model (Box Model / Модель коробки)**

Har bir HTML elementi to'rtburchak quti sifatida tasavvur qilinishi mumkin. Bu quti **box model** (box model / модель коробки) deb ataladi va quyidagi qismlardan iborat:

* **Tarkib (Content / Содержимое):** Elementning asosiy mazmuni (matn, rasm va boshqalar).
* **Ichki bo'sh joy (Padding / Внутренний отступ):** Tarkib atrofidagi bo'sh joy.
* **Chegara (Border / Граница):** Ichki bo'sh joy atrofidagi chegara.
* **Tashqi bo'sh joy (Margin / Внешний отступ):** Chegara atrofidagi bo'sh joy.

```
+---------------------+
|       Margin        |
|  +-----------------+  |
|  |     Border     |  |
|  |  +-------------+  |  |
|  |  |   Padding   |  |  |
|  |  |  +---------+  |  |  |
|  |  |  | Content |  |  |  |
|  |  |  +---------+  |  |  |
|  |  +-------------+  |  |
|  +-----------------+  |
|       Margin        |
+---------------------+
```

`margin`, `padding` va `border` xossalari yordamida siz elementning o'lchamini va boshqa elementlar bilan orasidagi masofani boshqarishingiz mumkin.

**Margin (Margin / Внешний отступ)**

`margin` xossa elementning tashqi chegarasidan tashqaridagi bo'sh joyni belgilaydi. `margin` xossasini quyidagi usullardan biri bilan o'rnatish mumkin:

* **Barcha tomonlar uchun bir xil qiymat:** `margin: 20px;`
* **Yuqori va pastki, chap va o'ng tomonlar uchun alohida qiymatlar:** `margin: 10px 20px;`
* **Yuqori, o'ng, pastki va chap tomonlar uchun alohida qiymatlar:** `margin: 5px 10px 15px 20px;`
* **Har bir tomon uchun alohida xossalar:** `margin-top: 5px;`, `margin-right: 10px;`, `margin-bottom: 15px;`, `margin-left: 20px;`

`margin` xossa uchun manfiy qiymatlar ham ishlatilishi mumkin. Manfiy qiymatlar elementni belgilangan yo'nalishda siljitadi.

**Padding (Padding / Внутренний отступ)**

`padding` xossa elementning ichki chegarasidan ichkaridagi bo'sh joyni belgilaydi. `padding` xossasini ham `margin` xossasi kabi turli xil usullar bilan o'rnatish mumkin.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 13: Margin va padding xossalarini qo'llang.**
    * HTML faylingizda bir nechta elementlar yarating (masalan, `<h1>`, `<p>`, `<div>`).
    * CSS faylingizda bu elementlarga `margin` va `padding` xossalarini qo'llang.
    * Turli xil qiymatlar bilan tajriba o'tkazing va elementlarning o'lchami va joylashuvi qanday o'zgarishini kuzating.

    ```css
    h1 {
      margin: 20px;
      padding: 10px;
      background-color: lightblue;
    }
    
    p {
      margin-top: 30px;
      padding-left: 15px;
      background-color: lightgreen;
    }
    
    div {
      margin: 0 50px; /* Yuqori va pastki margin 0, chap va o'ng margin 50px */
      padding: 20px 10px; /* Yuqori va pastki padding 20px, chap va o'ng padding 10px */
      background-color: lightcoral;
    }
    ```

* **Vazifa 14: Manfiy margin qiymatlarini qo'llang.**
    * Yuqoridagi vazifada yaratgan elementlardan biriga manfiy `margin` qiymatini qo'llang.
    * Elementning qanday siljishini kuzating.

    ```css
    h1 {
      margin: 20px;
      margin-top: -10px; /* Sarlavhani yuqoriga 10px ga siljitish */
      padding: 10px;
      background-color: lightblue;
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Rasmlar galereyasini yarating.**
    * HTML faylingizda bir nechta rasmlarni (`<img>`) qo'shing.
    * CSS faylingizda `margin` va `padding` xossalaridan foydalanib, rasmlar orasidagi bo'sh joyni sozlang.

    ```css
    img {
      width: 200px;
      margin: 10px;
    }
    ```

* **2-vazifa:  Navigatsiya menyusini yarating.**
    * HTML faylingizda navigatsiya menyusini yarating (`<nav>` va `<ul>`).
    * CSS faylingizda `margin` va `padding` xossalaridan foydalanib, menyu elementlari orasidagi bo'sh joyni sozlang.

    ```css
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
    }
    
    nav li {
      display: inline-block;
      margin: 0 10px;
      padding: 5px;
      background-color: lightblue;
    }
    ```

* **3-vazifa:  Shaxsiy veb-saytni stillashtiring.**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini CSS yordamida yanada stillashtiring.
    * `margin` va `padding` xossalaridan foydalanib, sahifa elementlari orasidagi bo'sh joyni sozlang.
</details>


<details>
   <summary>Joylashtirish (Positioning / Позиционирование)</summary>

**Joylashtirish (Positioning / Позиционирование)**

CSS da elementlarni sahifa bo'ylab joylashtirish uchun `position` xossa ishlatiladi. `position` xossa quyidagi qiymatlarni qabul qilishi mumkin:

* `static`: Element hujjat oqimida odatiy joylashtiriladi. Bu standart qiymat.
* `relative`: Element o'zining odatiy joylashuvidan nisbatan siljitiladi. `top`, `right`, `bottom` va `left` xossalari yordamida elementni siljitish mumkin.
* `absolute`: Element eng yaqin joylashtirilgan ota elementga nisbatan joylashtiriladi. Agar ota element `position: relative;` ga ega bo'lsa, element ota elementga nisbatan joylashtiriladi. Aks holda, element hujjatga nisbatan joylashtiriladi.
* `fixed`: Element brauzer oynasiga nisbatan joylashtiriladi va sahifa aylantirilganda ham o'z o'rnida qoladi.

`top`, `right`, `bottom` va `left` xossalari yordamida elementni joylashtirishni aniqroq boshqarish mumkin. Bu xossalar elementning yuqori, o'ng, pastki va chap chegaralaridan qancha masofada joylashishini belgilaydi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 15: `position: relative;` bilan ishlang.**
    * HTML faylingizda bir nechta elementlar yarating (masalan, `<div>`).
    * CSS faylingizda birinchi elementga `position: relative;` xossasini qo'llang.
    * `top`, `right`, `bottom` va `left` xossalaridan foydalanib, elementni turli yo'nalishlarda siljiting.

    ```css
    .quti1 {
      position: relative;
      top: 50px;
      left: 100px;
      background-color: lightblue;
    }
    ```

* **Vazifa 16: `position: absolute;` bilan ishlang.**
    * Yuqoridagi vazifada yaratgan elementlardan biriga `position: absolute;` xossasini qo'llang.
    * `top`, `right`, `bottom` va `left` xossalaridan foydalanib, elementni joylashtiring.
    * Ota elementga `position: relative;` xossasini qo'shib, elementning ota elementga nisbatan joylashishini kuzating.

    ```css
    .container {
      position: relative;
      width: 400px;
      height: 300px;
      border: 1px solid black;
    }
    
    .quti2 {
      position: absolute;
      top: 20px;
      right: 30px;
      background-color: lightgreen;
    }
    ```

* **Vazifa 17: `position: fixed;` bilan ishlang.**
    * HTML faylingizda biror element yarating (masalan, navigatsiya menyusi).
    * CSS faylingizda bu elementga `position: fixed;` xossasini qo'llang.
    * `top`, `right`, `bottom` va `left` xossalaridan foydalanib, elementni brauzer oynasining biror burchagiga joylashtiring.
    * Sahifani aylantirib, elementning o'z o'rnida qolishini kuzating.

    ```css
    nav {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      background-color: #333;
      color: white;
      padding: 10px;
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Suzuvchi tugma yarating.**
    * HTML faylingizda tugma (`<button>`) yarating.
    * CSS faylingizda `position: fixed;` xossasidan foydalanib, tugmani sahifaning pastki o'ng burchagiga joylashtiring.
    * Tugmani stillashtiring.

    ```css
    .floating-button {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #4CAF50; /* Yashil */
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    ```

* **2-vazifa:  Modal oyna yarating.**
    * HTML faylingizda modal oyna (modal window / модальное окно) yarating. Modal oyna odatda sahifaning ustida paydo bo'ladigan va foydalanuvchi uni yopmaguncha boshqa elementlar bilan ishlashga xalaqit beradigan oyna.
    * CSS faylingizda `position: fixed;` va `z-index` xossalaridan foydalanib, modal oynani joylashtiring va uni boshqa elementlar ustida ko'rsating.
    * JavaScript yordamida modal oynani ochish va yopish funksiyasini qo'shing.

    ```css
    .modal {
      display: none;
      position: fixed;
      z-index: 1; /* Modal oynani boshqa elementlar ustida ko'rsatish */
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0,0,0,0.4); /* Qora fon, shaffoflik bilan */
    }
    
    .modal-content {
      background-color: #fefefe;
      margin: 15% auto;
      padding: 20px;
      border: 1px solid #888;
      width: 80%;
    }
    ```

* **3-vazifa:  Shaxsiy veb-saytni joylashtirish bilan yaxshilang.**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini CSS yordamida yanada stillashtiring.
    * `position` xossa va `top`, `right`, `bottom`, `left` xossalaridan foydalanib, sahifa elementlarini turli xil joylarga joylashtiring.
</details>


<details>
   <summary>Flexbox (Flexbox / Flexbox)</summary>

**Flexbox (Flexbox / Flexbox)**

Flexbox - bu elementlarni bir qatorda yoki ustunda moslashuvchan tarzda joylashtirish imkonini beruvchi CSS moduli. Flexbox yordamida siz elementlarning o'lchamlarini, tartibini, hizalanishini va bo'sh joyni osongina boshqarishingiz mumkin. Bu, ayniqsa, responsiv dizayn yaratishda juda foydali.

Flexbox dan foydalanish uchun ota elementga `display: flex;` xossasini qo'llashingiz kerak. Keyin, bolalar elementlariga turli xil Flexbox xossalarini qo'llashingiz mumkin.

**Asosiy Flexbox xossalari:**

* **`flex-direction`:** Elementlarning joylashish yo'nalishini belgilaydi.
    * `row`: Elementlar gorizontal qatorda joylashadi (chapdan o'ngga).
    * `row-reverse`: Elementlar gorizontal qatorda joylashadi (o'ngdan chapga).
    * `column`: Elementlar vertikal ustunda joylashadi (yuqoridan pastga).
    * `column-reverse`: Elementlar vertikal ustunda joylashadi (pastdan yuqoriga).
* **`justify-content`:** Elementlarni asosiy o'q bo'ylab qanday hizalanishini belgilaydi.
    * `flex-start`: Elementlar konteynerning boshidan joylashadi.
    * `flex-end`: Elementlar konteynerning oxiridan joylashadi.
    * `center`: Elementlar konteynerning markazida joylashadi.
    * `space-between`: Elementlar orasidagi bo'sh joy teng taqsimlanadi.
    * `space-around`: Elementlarning ikki chetidagi bo'sh joy, elementlar orasidagi bo'sh joydan ikki baravar katta bo'ladi.
    * `space-evenly`: Barcha bo'sh joylar (elementlar orasidagi va chetlardagi) teng taqsimlanadi.
* **`align-items`:** Elementlarni ikkinchi darajali o'q bo'ylab qanday hizalanishini belgilaydi.
    * `flex-start`: Elementlar konteynerning boshidan hizalanadi.
    * `flex-end`: Elementlar konteynerning oxiridan hizalanadi.
    * `center`: Elementlar konteynerning markazida hizalanadi.
    * `stretch`: Elementlar konteynerning balandligiga cho'ziladi (standart qiymat).
* **`flex-wrap`:** Elementlar bir qatorga sig'masa, ularni qanday o'rashni belgilaydi.
    * `nowrap`: Elementlar o'ralmaydi (standart qiymat).
    * `wrap`: Elementlar yangi qatorga o'raladi.
    * `wrap-reverse`: Elementlar teskari tartibda yangi qatorga o'raladi.
* **`align-content`:** Bir nechta qatorlar bo'lganda, qatorlarni qanday hizalanishini belgilaydi. Xuddi `justify-content` kabi ishlaydi, lekin asosiy o'q o'rniga ikkinchi darajali o'q bo'ylab hizalaydi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 18: Flexbox bilan ustunlar yarating.**
    * HTML faylingizda bir nechta ustunlar yarating (`<div>`).
    * CSS faylingizda ota elementga `display: flex;` xossasini qo'llang.
    * `flex-direction`, `justify-content` va `align-items` xossalaridan foydalanib, ustunlarni turli xil usullar bilan joylashtiring.

    ```html
    <div class="container">
      <div class="ustun">Ustun 1</div>
      <div class="ustun">Ustun 2</div>
      <div class="ustun">Ustun 3</div>
    </div>
    ```

    ```css
    .container {
      display: flex;
      flex-direction: row; /* Ustunlarni gorizontal joylashtirish */
      justify-content: space-around; /* Ustunlar orasidagi bo'sh joyni teng taqsimlash */
      align-items: center; /* Ustunlarni vertikal markazga tekislash */
    }
    ```

* **Vazifa 19: Flexbox bilan menyu yarating.**
    * HTML faylingizda navigatsiya menyusi yarating (`<nav>` va `<ul>`).
    * CSS faylingizda `display: flex;` xossasini qo'llang va Flexbox xossalaridan foydalanib, menyu elementlarini gorizontal ravishda joylashtiring.

    ```css
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: space-between; /* Elementlarni orasidagi bo'sh joyni teng taqsimlash */
    }
    ```

* **Vazifa 20: Flexbox bilan elementlarni o'rang.**
    * HTML faylingizda bir nechta elementlar yarating (`<div>`).
    * CSS faylingizda `flex-wrap: wrap;` xossasini qo'llab, elementlarni yangi qatorga o'rashga majbur qiling.
    * `align-content` xossasidan foydalanib, qatorlarni turli xil usullar bilan hizalang.

    ```css
    .container {
      display: flex;
      flex-wrap: wrap;
      align-content: center; /* Qatorlarni vertikal markazga tekislash */
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Flexbox bilan murakkab tartib yarating.**
    * HTML faylingizda bir nechta elementlar yarating (sarlavhalar, xatboshilar, rasmlar, ro'yxatlar).
    * CSS faylingizda Flexbox xossalaridan foydalanib, bu elementlarni sahifa bo'ylab turli xil usullar bilan joylashtiring.

* **2-vazifa:  Flexbox bilan responsiv veb-sayt yarating.**
    * Oddiy veb-sayt yarating (masalan, "Men haqimda" sahifasi).
    * CSS faylingizda Flexbox va media so'rovlaridan foydalanib, saytni responsiv qiling.
    * Turli xil ekran o'lchamlarida saytning qanday ko'rinishini tekshiring.

* **3-vazifa:  Flexbox bilan rasm galereyasini yarating.**
    * HTML faylingizda rasm galereyasi yarating.
    * CSS faylingizda Flexbox xossalaridan foydalanib, rasmlarni chiroyli tarzda joylashtiring.
    * Rasmlar orasidagi bo'sh joyni sozlang.
    * Galereyani responsiv qiling.
</details>


<details>
   <summary>Media so'rovlar (Media Queries / Медиа-запросы)</summary>

**Media so'rovlar (Media Queries / Медиа-запросы)**

Responsiv veb-dizaynni yaratishda media so'rovlar muhim rol o'ynaydi. Media so'rovlar CSS qoidalarini ma'lum shartlar bajarilganda (masalan, ekran kengligi ma'lum bir qiymatdan kichik bo'lsa) qo'llash imkonini beradi.

Media so'rovlar quyidagi sintaksisga ega:

```css
@media (shart) {
  /* CSS qoidalari */
}
```

**Shartlar:**

* `max-width`: Ekran kengligi belgilangan qiymatdan kichik yoki teng bo'lganda stilni qo'llaydi.
* `min-width`: Ekran kengligi belgilangan qiymatdan katta yoki teng bo'lganda stilni qo'llaydi.
* `max-height`: Ekran balandligi belgilangan qiymatdan kichik yoki teng bo'lganda stilni qo'llaydi.
* `min-height`: Ekran balandligi belgilangan qiymatdan katta yoki teng bo'lganda stilni qo'llaydi.
* `orientation`: Qurilmaning orientatsiyasi (portret yoki landshaft) bo'yicha stilni qo'llaydi.

**Mantiqiy operatorlar:**

* `and`: Ikkala shart ham bajarilishi kerak.
* `or`: Shartlardan kamida bittasi bajarilishi kerak.
* `not`: Shart bajarilmasligi kerak.

**Misol:**

```css
/* Ekran kengligi 768px dan kichik bo'lganda */
@media (max-width: 768px) {
  body {
    background-color: lightblue;
  }

  h1 {
    font-size: 24px;
  }
}

/* Ekran kengligi 1024px dan katta bo'lganda va orientatsiya landshaft bo'lganda */
@media (min-width: 1024px) and (orientation: landscape) {
  .container {
    width: 80%;
  }
}
```

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 21: Media so'rovlar bilan responsiv menyu yarating.**
    * HTML faylingizda navigatsiya menyusi yarating (`<nav>` va `<ul>`).
    * CSS faylingizda media so'rovlaridan foydalanib, menyuni responsiv qiling.
    * Katta ekranlarda menyu elementlari gorizontal ravishda joylashsin.
    * Kichik ekranlarda menyu elementlari vertikal ravishda joylashsin.

    ```css
    /* Katta ekranlar uchun */
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: space-between;
    }

    /* Kichik ekranlar uchun */
    @media (max-width: 768px) {
      nav ul {
        flex-direction: column;
      }
    }
    ```

* **Vazifa 22: Media so'rovlar bilan rasmlarni moslashtiring.**
    * HTML faylingizga rasm qo'shing (`<img>`).
    * CSS faylingizda media so'rovlaridan foydalanib, rasmni turli ekran o'lchamlariga moslashtiring.
    * Katta ekranlarda rasm kengligi 50% bo'lsin.
    * Kichik ekranlarda rasm kengligi 100% bo'lsin.

    ```css
    img {
      width: 50%;
    }

    @media (max-width: 768px) {
      img {
        width: 100%;
      }
    }
    ```

* **Vazifa 23: Media so'rovlar bilan matn o'lchamini o'zgartiring.**
    * HTML faylingizda bir nechta sarlavhalar (`<h1>`, `<h2>`, `<h3>`) va xatboshilar (`<p>`) yarating.
    * CSS faylingizda media so'rovlaridan foydalanib, matn o'lchamini turli ekran o'lchamlariga moslashtiring.
    * Katta ekranlarda matn o'lchami katta bo'lsin.
    * Kichik ekranlarda matn o'lchami kichik bo'lsin.

    ```css
    h1 {
      font-size: 36px;
    }

    @media (max-width: 768px) {
      h1 {
        font-size: 24px;
      }
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Responsiv shaxsiy veb-sayt yarating.**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini responsiv qiling.
    * Media so'rovlaridan foydalanib, sahifa turli xil ekran o'lchamlarida to'g'ri ko'rinishini ta'minlang.

* **2-vazifa:  Responsiv mahsulot kartalari yarating.**
    * HTML da bir nechta mahsulot kartalari yarating.
    * CSS va media so'rovlaridan foydalanib, kartalarni responsiv qiling.
    * Katta ekranlarda kartalar yonma-yon joylashsin.
    * Kichik ekranlarda kartalar bir-birining ostiga joylashsin.

* **3-vazifa:  Responsiv forma yarating.**
    * HTML da forma yarating (masalan, aloqa formasi).
    * CSS va media so'rovlaridan foydalanib, formani responsiv qiling.
    * Katta ekranlarda forma maydonlari yonma-yon joylashsin.
    * Kichik ekranlarda forma maydonlari bir-birining ostiga joylashsin.
</details>


<details>
   <summary>Pseudo-klasslar (Pseudo-classes / Псевдоклассы)</summary>


**Pseudo-klasslar (Pseudo-classes / Псевдоклассы)**

Pseudo-klasslar CSS selektorlariga qo'shimcha tanlash imkoniyatlarini beradi. Ular elementning holatiga (masalan, sichqoncha ustiga qo'yilganda, faol bo'lganda) yoki hujjat daraxtidagi o'rniga (masalan, birinchi bola elementi) qarab stillarni qo'llashga imkon beradi.

Pseudo-klasslar selektorga ikki nuqta (`:`) bilan qo'shiladi.

Ba'zi foydali pseudo-klasslar:

* **Dinamik pseudo-klasslar:**
    * `:hover`: Sichqoncha elementi ustiga qo'yilganda stilni qo'llaydi.
    * `:active`: Element faol bo'lganda (masalan, bosilganda) stilni qo'llaydi.
    * `:focus`: Element fokuslanganda (masalan, matn maydoniga yozish boshlanganda) stilni qo'llaydi.
* **Tartib pseudo-klasslari:**
    * `:first-child`: Ota elementning birinchi bola elementiga stilni qo'llaydi.
    * `:last-child`: Ota elementning oxirgi bola elementiga stilni qo'llaydi.
    * `:nth-child(n)`: Ota elementning n-chi bola elementiga stilni qo'llaydi.
    * `:nth-of-type(n)`: Ota elementning ma'lum turdagi n-chi bola elementiga stilni qo'llaydi.

**Misol:**

```css
/* Havolalar */
a:link { color: blue; } /* Oddiy havola */
a:visited { color: purple; } /* Tashrif buyurilgan havola */
a:hover { color: red; } /* Sichqoncha ustiga qo'yilganda */
a:active { color: yellow; } /* Bosilganda */

/* Ro'yxat elementlari */
li:first-child { font-weight: bold; } /* Birinchi element */
li:nth-child(2) { color: red; } /* Ikkinchi element */
```

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 24: Havolalarni stillashtiring.**
    * HTML faylingizda bir nechta havolalar yarating (`<a>`).
    * CSS faylingizda `:link`, `:visited`, `:hover` va `:active` pseudo-klasslaridan foydalanib, havolalarni turli holatlarda stillashtiring.

    ```css
    a:link {
      color: blue;
      text-decoration: none;
    }
    
    a:visited {
      color: purple;
    }
    
    a:hover {
      color: red;
      text-decoration: underline;
    }
    
    a:active {
      color: orange;
    }
    ```

* **Vazifa 25: Ro'yxat elementlarini stillashtiring.**
    * HTML faylingizda ro'yxat yarating (`<ul>` yoki `<ol>`).
    * CSS faylingizda `:first-child`, `:last-child` va `:nth-child(n)` pseudo-klasslaridan foydalanib, ro'yxat elementlarini stillashtiring.

    ```css
    li:first-child {
      font-weight: bold;
    }
    
    li:last-child {
      font-style: italic;
    }
    
    li:nth-child(3) {
      color: red;
    }
    ```

* **Vazifa 26: Tugmani stillashtiring.**
    * HTML faylingizda tugma yarating (`<button>`).
    * CSS faylingizda `:hover`, `:active` va `:focus` pseudo-klasslaridan foydalanib, tugmani stillashtiring.

    ```css
    button:hover {
      background-color: #45a049; /* To'qroq yashil */
    }
    
    button:active {
      background-color: #3e8e41; /* Yana to'qroq yashil */
      box-shadow: 0 5px #666;
      transform: translateY(4px);
    }
    
    button:focus {
      outline: none; /* Fokuslanganda standart chegarani olib tashlash */
      box-shadow: 0 0 5px blue;
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Jadvalni stillashtiring.**
    * HTML faylingizda jadval yarating (`<table>`).
    * CSS faylingizda pseudo-klasslardan foydalanib, jadvalning birinchi va oxirgi qatorlarini, shuningdek, juft va toq qatorlarini turli xil stillarda ajratib ko'rsating.

    ```css
    tr:first-child {
      background-color: #f2f2f2;
    }
    
    tr:last-child {
      font-weight: bold;
    }
    
    tr:nth-child(even) {
      background-color: #f9f9f9;
    }
    ```

* **2-vazifa:  Shaklni stillashtiring.**
    * HTML faylingizda shakl yarating (`<form>`).
    * CSS faylingizda pseudo-klasslardan foydalanib, shakl maydonlarini (`<input>`, `<textarea>`) fokuslanganda, hover qilinganda va xatolik yuz berganda stillashtiring.

    ```css
    input:focus, textarea:focus {
      border-color: blue;
    }
    
    input:hover, textarea:hover {
      background-color: #f5f5f5;
    }
    
    input:invalid {
      border-color: red;
    }
    ```

* **3-vazifa:  Dropdown menyu yarating.**
    * HTML faylingizda dropdown menyu yarating.
    * CSS faylingizda pseudo-klasslardan foydalanib, menyu elementlarini hover qilinganda stillashtiring.
    * Menyuni ochish va yopish uchun JavaScript dan foydalaning.

    ```css
    .dropdown:hover .dropdown-content {
      display: block;
    }
    
    .dropdown-content a:hover {
      background-color: #ddd;
    }
    ```
</details>


<details>
   <summary>Display xossasi (Display Property / Свойство отображения)</summary>


**Display xossasi (Display Property / Свойство отображения)**

`display` xossasi elementning ko'rinish turini belgilaydi. Bu xossa yordamida elementni blok, inline yoki umuman ko'rinmas qilish mumkin.

`display` xossasining ba'zi qiymatlari:

* `block`: Element yangi qatorga joylashadi va konteynerning to'liq kengligini egallaydi. Masalan, `<h1>`, `<p>`, `<div>` teglar standart ravishda `display: block;` ga ega.
* `inline`: Element yangi qatorga joylashmaydi va faqat o'z mazmuni uchun kerakli kenglikni egallaydi. Masalan, `<span>`, `<a>`, `<strong>` teglar standart ravishda `display: inline;` ga ega.
* `inline-block`: Element inline element kabi joylashadi, lekin blok element kabi kenglik, balandlik, margin va padding xossalariga ega bo'ladi.
* `none`: Elementni yashiradi. Element sahifa tartibida joy egallamaydi va ko'rinmaydi.

**Visibility xossasi (Visibility Property / Свойство видимости)**

`visibility` xossasi ham elementni yashirish uchun ishlatiladi, lekin `display: none;` dan farqli o'laroq, element sahifa tartibida joy egallaydi, faqat ko'rinmaydi.

`visibility` xossasining qiymatlari:

* `visible`: Element ko'rinadi. Bu standart qiymat.
* `hidden`: Element ko'rinmaydi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 27: `display` xossasini qo'llang.**
    * HTML faylingizda bir nechta elementlar yarating (masalan, `<h1>`, `<p>`, `<div>`, `<span>`).
    * CSS faylingizda bu elementlarga `display` xossasining turli qiymatlarini qo'llang.
    * Elementlarning joylashuvi va o'lchamlari qanday o'zgarishini kuzating.

    ```css
    h1 {
      display: inline; /* Sarlavhani inline elementga aylantirish */
    }
    
    span {
      display: block; /* Spanni blok elementga aylantirish */
      width: 200px;
      background-color: lightblue;
    }
    
    div {
      display: inline-block; /* Divni inline-block elementga aylantirish */
      margin: 10px;
      padding: 5px;
      border: 1px solid black;
    }
    ```

* **Vazifa 28: `visibility` xossasini qo'llang.**
    * HTML faylingizda bir nechta elementlar yarating.
    * CSS faylingizda bu elementlardan birini `visibility: hidden;` yordamida yashiring.
    * Elementning sahifa tartibida joy egallab turganini, lekin ko'rinmasligini kuzating.

    ```css
    p {
      visibility: hidden;
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Navigatsiya menyusini yarating.**
    * HTML faylingizda navigatsiya menyusi yarating (`<nav>` va `<ul>`).
    * CSS faylingizda `display: inline-block;` xossasidan foydalanib, menyu elementlarini gorizontal ravishda joylashtiring.
    * Menyuni stillashtiring.

    ```css
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
    }
    
    nav li {
      display: inline-block;
      margin: 0 10px;
      padding: 5px;
      background-color: lightblue;
    }
    ```

* **2-vazifa:  Elementlarni yashiring va ko'rsating.**
    * HTML faylingizda bir nechta elementlar yarating.
    * CSS faylingizda `display: none;` va `visibility: hidden;` xossalaridan foydalanib, ba'zi elementlarni yashiring.
    * JavaScript yordamida tugma bosilganda yashiringan elementlarni ko'rsating va ko'rinib turgan elementlarni yashiring.

* **3-vazifa:  Shaxsiy veb-saytni stillashtiring.**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini CSS yordamida yanada stillashtiring.
    * `display` xossasidan foydalanib, ba'zi elementlarning ko'rinish turini o'zgartiring.
    * `visibility` xossasidan foydalanib, ba'zi elementlarni yashiring.
</details>

<details>
   <summary></summary>
</details>
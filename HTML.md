<!-- HTML 1 -->
<details>
   <summary>1-modul: Front-end asoslari va asosiy vositalar</summary>


**HTML asoslari (HTML Essentials / Основы HTML)**

**Dars uchun qo'llanma**

**HTML nima? (What is HTML? / Что такое HTML?)**

HTML (HyperText Markup Language / Язык гипертекстовой разметки) veb-sahifalarni yaratish uchun ishlatiladigan tildir. U brauzerga veb-sahifaning tuzilishini va tarkibini tushuntirish uchun teglar (tags / теги) dan foydalanadi. HTML hujjatlari oddiy matn fayllari bo'lib, `.html` yoki `.htm` kengaytmasiga ega.

**Asosiy HTML tuzilishi (Basic HTML Structure / Основная структура HTML)**

Har bir HTML hujjati quyidagi asosiy tuzilishga ega:

```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <title>Sahifa sarlavhasi</title>
</head>
<body>

</body>
</html>
```

* `<!DOCTYPE html>`: Bu teg brauzerga HTML5 standartidan foydalanayotganingizni bildiradi.
* `<html lang="uz">`: Bu hujjatning asosiy tegi (root element / корневой элемент). `lang` atributi sahifaning tilini belgilaydi (bu yerda "uz" o'zbek tilini bildiradi).
* `<head>`: Bu qismda sahifa haqidagi meta-ma'lumotlar, sarlavha va boshqa ko'rinmas elementlar saqlanadi.
    * `<meta charset="UTF-8">`: Bu teg matn kodlashni belgilaydi. UTF-8 kodlash turli tillardagi belgilarni qo'llab-quvvatlaydi.
    * `<title>`: Bu teg brauzer yorlig'ida ko'rinadigan sahifa sarlavhasini (title / заголовок) belgilaydi.
* `<body>`: Bu qismda sahifaning ko'rinadigan tarkibi joylashtiriladi.

**HTML teglar (HTML Tags / Теги HTML)**

HTML teglar veb-sahifaning turli elementlarini belgilash uchun ishlatiladi. Teglar odatda juft bo'lib keladi: ochilish tegi (`<tag>`) va yopilish tegi (`</tag>`). Ba'zi teglar esa yakka holda ishlatiladi (masalan, `<img>`).

Keling, ba'zi umumiy HTML teglarini ko'rib chiqaylik:

* **Sarlavhalar (Headings / Заголовки):** `<h1>` dan `<h6>` gacha (turli sarlavha darajalari uchun)
   ```html
   <h1>Bu asosiy sarlavha</h1>
   <h2>Bu kichik sarlavha</h2>
   ```
* **Xatboshilar (Paragraphs / Абзацы):** `<p>`
   ```html
   <p>Bu matn xatboshisi.</p>
   ```
* **Havolalar (Links / Ссылки):** `<a href="url">Havola matni</a>`
   ```html
   <a href="https://www.google.com">Google ga o'ting</a>
   ```
* **Rasmlar (Images / Изображения):** `<img src="image.jpg" alt="Rasm tavsifi">`
   ```html
   <img src="mypicture.jpg" alt="Mening rasmim">
   ```
* **Qator uzilishlari (Line Breaks / Разрывы строк):** `<br>`
* **Bo'limlar (Divisions / Разделы):** `<div>` (elementlarni guruhlash uchun ishlatiladi)
* **Tartibsiz ro'yxatlar (Unordered Lists / Неупорядоченные списки):** `<ul>`, `<li>`
   ```html
   <ul>
       <li>Birinchi element</li>
       <li>Ikkinchi element</li>
   </ul>
   ```
* **Tartiblangan ro'yxatlar (Ordered Lists / Упорядоченные списки):** `<ol>`, `<li>`
   ```html
   <ol>
       <li>Birinchi element</li>
       <li>Ikkinchi element</li>
   </ol>
   ```


**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 1: To'liq HTML hujjatini yarating va asosiy teglarni qo'shing.**
    * Yangi fayl yarating va uni `index.html` deb nomlang.
    * Kod muharriringizda faylni oching va asosiy HTML tuzilishini yozing: `<!DOCTYPE html>`, `<html lang="uz">`, `<head>`, `<title>`, `<meta charset="UTF-8">` va `<body>` teglarini qo'shing.
    * `<title>` tegi ichida sahifangiz uchun sarlavha yozing (masalan, "Mening birinchi veb-sahifam").
    * `<body>` teglari ichida quyidagi elementlarni qo'shing:
        * `<h1>` tegi bilan asosiy sarlavha (masalan, "Salom, Dunyo!").
        * `<h2>` tegi bilan kichik sarlavha (masalan, "Bu mening birinchi veb-sahifam").
        * Ikkita `<p>` tegi bilan ikkita xatboshi. Har bir xatboshida bir nechta jumla yozing.
    * Faylni saqlang va brauzerda oching. Brauzer oynasida yaratgan sahifangizni ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening birinchi veb-sahifam</title>
    </head>
    <body>
        <h1>Salom, Dunyo!</h1>
        <h2>Bu mening birinchi veb-sahifam</h2>
        <p>Bu birinchi xatboshi. Bu yerda bir nechta jumlalar yozilgan.</p>
        <p>Bu ikkinchi xatboshi. Bu yerda ham bir nechta jumlalar yozilgan.</p>
    </body>
    </html>
    ```

* **Vazifa 2: Rasm va havolalarni qo'shing.**
    * Yuqorida yaratgan HTML faylingizni oching.
    * `<img>` tegi yordamida sahifaga rasm qo'shing. `src` atributida rasmning manzilini ko'rsating. `alt` atributida rasmning qisqacha tavsifini yozing.
    * `<a>` (anchor) tegi yordamida veb-sahifaga havola qo'shing. `href` atributida havolaning manzilini ko'rsating (masalan, "[https://www.google.com](https://www.google.com)"). Havola matnini teglar orasiga yozing (masalan, "Google").
    * Faylni saqlang va brauzerda yangilang. Endi sahifangizda rasm va havola ko'rinishi kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening birinchi veb-sahifam</title>
    </head>
    <body>
        <h1>Salom, Dunyo!</h1>
        <h2>Bu mening birinchi veb-sahifam</h2>
        <p>Bu birinchi xatboshi. Bu yerda bir nechta jumlalar yozilgan.</p>
        <p>Bu ikkinchi xatboshi. Bu yerda ham bir nechta jumlalar yozilgan.</p>
        <img src="rasm.jpg" alt="Chiroyli rasm">
        <a href="https://www.google.com">Google</a>
    </body>
    </html>
    ```

* **Vazifa 3: Ro'yxatlarni qo'shing.**
    * Yuqoridagi HTML faylingizga tartiblangan va tartibsiz ro'yxatlarni qo'shing.
    * Tartibsiz ro'yxat uchun `<ul>` va `<li>` teglaridan foydalaning.
    * Tartiblangan ro'yxat uchun `<ol>` va `<li>` teglaridan foydalaning.
    * Har bir ro'yxatga kamida 3 ta element qo'shing.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening birinchi veb-sahifam</title>
    </head>
    <body>
        <h1>Salom, Dunyo!</h1>
        <h2>Bu mening birinchi veb-sahifam</h2>
        <p>Bu birinchi xatboshi. Bu yerda bir nechta jumlalar yozilgan.</p>
        <p>Bu ikkinchi xatboshi. Bu yerda ham bir nechta jumlalar yozilgan.</p>
        <img src="rasm.jpg" alt="Chiroyli rasm">
        <a href="https://www.google.com">Google</a>
    
        <h3>Sevimli ranglarim</h3>
        <ul>
            <li>Qizil</li>
            <li>Yashil</li>
            <li>Ko'k</li>
        </ul>
    
        <h3>Sevimli mashg'ulotlarim</h3>
        <ol>
            <li>Kitob o'qish</li>
            <li>Musiqa tinglash</li>
            <li>Sayohat qilish</li>
        </ol>
    </body>
    </html>
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa: "Mening sevimli mashg'ulotlarim"**
    * "Mening sevimli mashg'ulotlarim" (My favorite hobbies / Мои любимые хобби) deb nomlangan veb-sahifa yarating.
    * Sevimli mashg'ulotlaringiz haqida ma'lumot beruvchi sarlavhalar va xatboshilar yozing.
    * Har bir mashg'ulot uchun alohida bo'lim (`<div>`) yarating.
    * Bo'limlarga sarlavhalar (`<h2>` yoki `<h3>`) qo'shing.
    * Har bir bo'limda mashg'ulot haqida batafsil ma'lumot bering, rasmlar qo'shing va tegishli veb-saytlarga havolalar bering.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening sevimli mashg'ulotlarim</title>
    </head>
    <body>
        <h1>Mening sevimli mashg'ulotlarim</h1>
    
        <div>
            <h2>Kitob o'qish</h2>
            <p>Menga turli xil kitoblar o'qish yoqadi. Ayniqsa fantastika va detektiv janridagi kitoblarni yoqtiraman.</p>
            <img src="kitob.jpg" alt="Kitob">
        </div>
    
        <div>
            <h2>Musiqa tinglash</h2>
            <p>Men turli xil musiqalarni tinglayman. Klassik musiqadan tortib, zamonaviy pop musiqagacha.</p>
            <a href="https://spotify.com">Spotify</a> da musiqa tinglashni yoqtiraman.
        </div>
    
    </body>
    </html>
    ```

* **2-vazifa:  "Mening oilam"**
    * "Mening oilam" (My family / Моя семья) deb nomlangan veb-sahifa yarating.
    * Oila a'zolaringiz haqida ma'lumot bering.
    * Har bir oila a'zosi uchun alohida bo'lim (`<div>`) yarating.
    * Bo'limlarga sarlavhalar (`<h2>` yoki `<h3>`) qo'shing va oila a'zolaringizning ismlarini yozing.
    * Har bir bo'limda oila a'zolaringiz haqida qisqacha ma'lumot bering, rasmlar qo'shing.
    * Oila a'zolaringizning sevimli mashg'ulotlari yoki qiziqishlari haqida ro'yxatlar (`<ul>` yoki `<ol>`) yarating.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening oilam</title>
    </head>
    <body>
        <h1>Mening oilam</h1>
    
        <div>
            <h2>Otam</h2>
            <img src="otam.jpg" alt="Otam">
            <p>Otamning ismi ... . U ... kasbida ishlaydi.</p>
        </div>
    
        <div>
            <h2>Onam</h2>
            <img src="onam.jpg" alt="Onam">
            <p>Onamning ismi ... . U ... kasbida ishlaydi.</p>
        </div>
    
    </body>
    </html>
    ```

* **3-vazifa:  "Mening maktabim"**
    * "Mening maktabim" (My school / Моя школа) deb nomlangan veb-sahifa yarating.
    * Maktabingiz haqida ma'lumot bering.
    * Maktabingizning rasmini qo'shing.
    * Maktabingizdagi sevimli fanlaringiz ro'yxatini tuzing.
    * Maktabingizning veb-saytiga havola qo'shing (agar mavjud bo'lsa).
    * Maktabingiz haqida qo'shimcha ma'lumotlarni (manzili, telefon raqami, email manzili) alohida bo'limda ko'rsating.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening maktabim</title>
    </head>
    <body>
        <h1>Mening maktabim</h1>
        <img src="maktab.jpg" alt="Maktabim">
        <p>Men ... maktabida o'qiyman. Bu maktab ... da joylashgan.</p>
    
        <h2>Sevimli fanlarim</h2>
        <ol>
            <li>Matematika</li>
            <li>Fizika</li>
            <li>Informatika</li>
        </ol>
    
        <a href="https://maktab.uz">Maktab veb-sayti</a>
    
    </body>
    </html>
    ```
</details>

<!-- 2 -->
<details>
   <summary>Jadvallar (Tables / Таблицы)</summary>

**Jadvallar (Tables / Таблицы)**

Jadvallar ma'lumotlarni satr va ustunlarga ajratilgan holda tuzilgan ko'rinishda taqdim etish uchun ishlatiladi. HTML da jadvallarni yaratish uchun quyidagi teglar ishlatiladi:

* `<table>`: Jadvalni belgilaydi.
* `<tr>`: Jadvaldagi satrni (table row / строка таблицы) belgilaydi.
* `<td>`: Jadvaldagi katakchani (table data / ячейка данных) belgilaydi.
* `<th>`: Jadvaldagi sarlavha katakchasini (table header / ячейка заголовка) belgilaydi (odatda qalin shriftda ko'rsatiladi).

```html
<table>
  <tr>
    <th>Ism</th>
    <th>Yoshi</th>
  </tr>
  <tr>
    <td>Ali</td>
    <td>20</td>
  </tr>
  <tr>
    <td>Vali</td>
    <td>25</td>
  </tr>
</table>
```

**Formlar (Forms / Формы)**

Formlar foydalanuvchidan ma'lumotlarni olish uchun ishlatiladi. HTML da formlarni yaratish uchun quyidagi teglar ishlatiladi:

* `<form>`: Formani belgilaydi.
* `<input>`: Turli xil kiritish maydonlarini (input fields / поля ввода) yaratish uchun ishlatiladi (matn, parol, radio tugmalari, checkboxlar va boshqalar).
* `<label>`: Kiritish maydonlari uchun yorliqlar (labels / метки) yaratish uchun ishlatiladi.
* `<textarea>`: Ko'p qatorli matn maydonlarini yaratish uchun ishlatiladi.
* `<select>`: Tanlash ro'yxatini (dropdown list / выпадающий список) yaratish uchun ishlatiladi.
* `<button>`: Tugmani (button / кнопка) yaratish uchun ishlatiladi.

```html
<form>
  <label for="ism">Ismingiz:</label>
  <input type="text" id="ism" name="ism">

  <label for="email">Emailingiz:</label>
  <input type="email" id="email" name="email">

  <button type="submit">Yuborish</button>
</form>
```

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 4: Jadval yaratish va ma'lumotlarni kiritish**

    * `table` tegi yordamida jadval yarating.
    * Jadvalga 3 ta ustun va 4 ta qator qo'shing.
    * Birinchi qatorni sarlavha qatori sifatida belgilang va unga "Ism", "Familiya", "Yoshi" sarlavhalarini qo'shing.
    * Qolgan qatorlarga o'zingiz bilgan odamlar haqida ma'lumotlarni kiriting (ixtiyoriy).
    * Jadvalga `border` atributi qo'shib, katakchalar orasidagi chegaralarni ko'rsating.
    * `cellpadding` va `cellspacing` atributlari yordamida katakchalar orasidagi bo'sh joyni o'zgartirib ko'ring.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Jadval yaratish</title>
    </head>
    <body>
    
      <table border="1" cellpadding="10" cellspacing="0">
        <tr>
          <th>Ism</th>
          <th>Familiya</th>
          <th>Yoshi</th>
        </tr>
        <tr>
          <td>Ali</td>
          <td>Valiyev</td>
          <td>25</td>
        </tr>
        <tr>
          <td>Olim</td>
          <td>Akbarov</td>
          <td>30</td>
        </tr>
        <tr>
          <td>Fotima</td>
          <td>Umarova</td>
          <td>22</td>
        </tr>
      </table>
    
    </body>
    </html>
    ```

* **Vazifa 5:  Anketa formasi yaratish**

    * `<form>` tegi yordamida anketa formasi yarating.
    * Formada quyidagi maydonlarni yarating:
        * Ism (`<input type="text">`)
        * Familiya (`<input type="text">`)
        * Email (`<input type="email">`)
        * Telefon raqami (`<input type="tel">`)
        * Jinsi (`<input type="radio">` tugmalari yordamida "Erkak" va "Ayol" variantlarini yarating)
        * Manzil (`<textarea>`)
    * Har bir maydon uchun `<label>` tegi yordamida yorliq qo'shing.
    * Formada "Yuborish" tugmasi (`<button type="submit">`) bo'lsin.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Anketa formasi</title>
    </head>
    <body>
    
      <form>
        <label for="ism">Ism:</label>
        <input type="text" id="ism" name="ism"><br><br>
    
        <label for="familiya">Familiya:</label>
        <input type="text" id="familiya" name="familiya"><br><br>
    
        <label for="email">Email:</label>
        <input type="email" id="email" name="email"><br><br>
    
        <label for="tel">Telefon raqami:</label>
        <input type="tel" id="tel" name="tel"><br><br>
    
        <label for="jinsi">Jinsi:</label>
        <input type="radio" id="erkak" name="jinsi" value="erkak">
        <label for="erkak">Erkak</label>
        <input type="radio" id="ayol" name="jinsi" value="ayol">
        <label for="ayol">Ayol</label><br><br>
    
        <label for="manzil">Manzil:</label>
        <textarea id="manzil" name="manzil"></textarea><br><br>
    
        <button type="submit">Yuborish</button>
      </form>
    
    </body>
    </html>
    ```

* **Vazifa 6: Tanlash ro'yxati va tugmalar**

    * `<select>` tegi yordamida tanlash ro'yxati yarating.
    * Ro'yxatda kamida 3 ta variant (`<option>`) bo'lsin.
    * Turli xil tugmalar (`<button>`) yarating va ularga turli xil atributlar (`type`, `disabled`) qo'shing.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Tanlash ro'yxati va tugmalar</title>
    </head>
    <body>
    
      <select>
        <option value="olma">Olma</option>
        <option value="banan">Banan</option>
        <option value="anor">Anor</option>
      </select>
      <br><br>
    
      <button type="submit">Yuborish</button>
      <button type="reset">Tozalash</button>
      <button type="button" disabled>Bosilmaydi</button>
    
    </body>
    </html>
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  "Mening sevimli kitoblarim"**
    * "Mening sevimli kitoblarim" (My favorite books / Мои любимые книги) deb nomlangan veb-sahifa yarating.
    * Sevimli kitoblaringiz ro'yxatini jadval (`<table>`) ko'rinishida yarating. 
        * Jadvalda quyidagi ustunlar bo'lsin: Kitob nomi, Muallif, Nashr yili, Janr.
        * Kamida 5 ta kitob haqida ma'lumot qo'shing.
    * Har bir kitob uchun alohida qator (`<tr>`) yarating.
    * Kitob nomlari uchun `<th>` (table header) tegini ishlating.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Mening sevimli kitoblarim</title>
    </head>
    <body>
      <h1>Mening sevimli kitoblarim</h1>
    
      <table border="1">
        <tr>
          <th>Kitob nomi</th>
          <th>Muallif</th>
          <th>Nashr yili</th>
          <th>Janr</th>
        </tr>
        <tr>
          <td>O'tkan kunlar</td>
          <td>Abdulla Qodiriy</td>
          <td>1926</td>
          <td>Roman</td>
        </tr>
        <tr>
          <td>Mehrobdan chayon</td>
          <td>Abdulla Qodiriy</td>
          <td>1929</td>
          <td>Roman</td>
        </tr>
        </table>
    
    </body>
    </html>
    ```

* **2-vazifa:  "Ro'yxatdan o'tish formasi"**
    * Foydalanuvchilar ro'yxatdan o'tishi uchun forma yarating.
    * Formada quyidagi maydonlarni yarating:
        * Foydalanuvchi nomi (`<input type="text">`)
        * Email (`<input type="email">`)
        * Parol (`<input type="password">`)
        * Parolni tasdiqlash (`<input type="password">`)
        * Tug'ilgan sana (`<input type="date">`)
        * Jinsi (`<input type="radio">` tugmalari yordamida)
        * Qiziqishlar (`<input type="checkbox">` yordamida bir nechta variantlarni tanlash)
        * "Ro'yxatdan o'tish" tugmasi (`<button type="submit">`)
    * Har bir maydon uchun tegishli yorliq (`<label>`) qo'shing.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Ro'yxatdan o'tish formasi</title>
    </head>
    <body>
      <h1>Ro'yxatdan o'tish</h1>
    
      <form>
        <label for="username">Foydalanuvchi nomi:</label>
        <input type="text" id="username" name="username"><br><br>
    
        <label for="email">Email:</label>
        <input type="email" id="email" name="email"><br><br>
    
        <button type="submit">Ro'yxatdan o'tish</button>
      </form>
    
    </body>
    </html>
    ```

* **3-vazifa:  "Restoran menyusi"**
    * Restoran menyusi uchun veb-sahifa yarating.
    * Menyuni jadval (`<table>`) ko'rinishida yarating.
    * Jadvalda quyidagi ustunlar bo'lsin: Taom nomi, Narxi, Tavsif.
    * Turli xil taomlarni (masalan, salatlar, sho'rvalar, asosiy taomlar, desertlar) alohida bo'limlarda ko'rsating.
    * Har bir bo'lim uchun sarlavha (`<h2>` yoki `<h3>`) qo'shing.
    * Rasmlarni qo'shishni unutmang.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Restoran menyusi</title>
    </head>
    <body>
      <h1>Restoran menyusi</h1>
    
      <h2>Salatlar</h2>
      <table border="1">
        <tr>
          <th>Nom</th>
          <th>Narx</th>
          <th>Tavsif</th>
        </tr>
        <tr>
          <td>Sezar salati</td>
          <td>15000 so'm</td>
          <td>Tovuq go'shti, parmezan pishlog'i va kruto'nlar bilan</td>
        </tr>
        </table>
    
      <h2>Sho'rvalar</h2>
      <table border="1">
        </table>
    
      </body>
    </html>
    ```

</details>

<details>
   <summary>HTML Atributlari (HTML Attributes / Атрибуты HTML)</summary>


**HTML Atributlari (HTML Attributes / Атрибуты HTML)**

HTML teglar qo'shimcha ma'lumotlarni o'z ichiga olishi mumkin. Bu ma'lumotlar **atributlar** (attributes / атрибуты) yordamida beriladi. Atributlar tegning ochilish qismida yoziladi va `nom="qiymat"` formatida bo'ladi.

Masalan, rasm tegida (`<img>`) `src` atributi rasm faylining manzilini, `alt` atributi esa rasmning tavsifini belgilaydi:

```html
<img src="rasm.jpg" alt="Chiroyli rasm">
```

Ba'zi umumiy HTML atributlari:

* `class`: Elementga CSS stillarini qo'llash uchun ishlatiladi.
* `id`: Elementga noyob identifikator beradi.
* `style`: Elementga inline stillarni qo'llash uchun ishlatiladi.
* `href`: Havola tegi (`<a>`) uchun havolaning manzilini belgilaydi.
* `src`: Rasm tegi (`<img>`) va boshqa media teglar (masalan, `<audio>`, `<video>`) uchun fayl manzilini belgilaydi.
* `alt`: Rasm tegi (`<img>`) uchun rasmning tavsifini belgilaydi.
* `width`: Elementning kengligini belgilaydi.
* `height`: Elementning balandligini belgilaydi.
* `title`: Element haqida qo'shimcha ma'lumotni ko'rsatish uchun ishlatiladi (masalan, sichqoncha ustiga qo'yilganda paydo bo'ladigan matn).


**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 7: Rasmlarga atributlar qo'shing va ularni stillashtiring**
    * Oldingi vazifalarda yaratgan HTML faylingizni oching.
    * `<img>` tegi yordamida sahifaga rasm qo'shing.
    * Rasmga `width` va `height` atributlarini qo'shib, uning o'lchamlarini o'zgartiring.
    * `alt` atributiga rasmning tavsifini yozing.
    * `style` atributi yordamida rasmga chegara (`border`) qo'shing va rasmni hizalang (`text-align`).
    * Faylni saqlang va brauzerda yangilang. Rasmning o'lchami, chegarasi va hizalanishi o'zgarganini ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening birinchi veb-sahifam</title>
    </head>
    <body>
        <img src="rasm.jpg" alt="Tog' manzarasi" width="500" height="300" 
             style="border: 5px solid black; display: block; margin-left: auto; margin-right: auto;"> 
    </body>
    </html>
    ```

* **Vazifa 8: Havolalarga atributlar qo'shing va ularni stillashtiring**
    * Sahifaga bir nechta havolalar (`<a>`) qo'shing.
    * Har bir havolaga `title` atributi qo'shib, havola haqida qo'shimcha ma'lumot bering. Masalan, havola qaysi saytga olib borishini yozing.
    * `style` atributi yordamida havolalarning rangini va chizilgan chiziqni o'zgartiring.
    * Faylni saqlang va brauzerda yangilang. Sichqonchani havolaning ustiga qo'yganingizda, `title` atributida yozgan matningiz paydo bo'lishini va stillar qo'llanilganini ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening birinchi veb-sahifam</title>
    </head>
    <body>
        <a href="https://kun.uz" title="Kun.uz yangiliklar sayti" style="color: red; text-decoration: none;">Kun.uz</a><br>
        <a href="https://wikipedia.org" title="Vikipediya - erkin ensiklopediya" style="color: green; text-decoration: underline;">Vikipediya</a>
    </body>
    </html>
    ```

* **Vazifa 9: Jadvalga atributlar qo'shing**
    * Oldingi "Jadvallar" bo'limida yaratilgan jadvalga atributlar qo'shing.
    * `border` atributi yordamida jadvalga chegara qo'shing.
    * `cellpadding` va `cellspacing` atributlari yordamida katakchalar orasidagi bo'sh joyni o'zgartiring.
    * `width` va `height` atributlari yordamida jadvalning o'lchamlarini o'rnating.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Jadval yaratish</title>
    </head>
    <body>
    
      <table border="1" cellpadding="10" cellspacing="5" width="500" height="200">
        <tr>
          <th>Ism</th>
          <th>Yoshi</th>
        </tr>
        <tr>
          <td>Ali</td>
          <td>20</td>
        </tr>
        <tr>
          <td>Vali</td>
          <td>25</td>
        </tr>
      </table>
    
    </body>
    </html>
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa: Shaxsiy veb-saytni atributlar bilan yaxshilang**
    * "Men haqimda" sahifangizga atributlar qo'shib, uni yanada yaxshilang.
    * Rasmlarga `width`, `height` va `alt` atributlarini qo'shing.
    * Havolalarga `title` atributi qo'shing.
    * Tegishli elementlarga `class` va `id` atributlarini qo'shing.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Men haqimda</title>
    </head>
    <body>
        <h1 id="main-heading">Men haqimda</h1>
        <img src="mening_rasmim.jpg" alt="Mening rasmim" width="200" height="300">
        <p>Mening ismim ... . Men ... yoshdaman.</p>
        <a href="https://sevimli_saytim.uz" title="Sevimli saytim">Sevimli saytimga tashrif buyuring</a>
    </body>
    </html>
    ```

* **2-vazifa:  Dars jadvali**
    * Dars jadvalingizni jadval (`<table>`) ko'rinishida yarating.
    * Jadvalda quyidagi ustunlar bo'lsin: Dars vaqti, Dushanba, Seshanba, Chorshanba, Payshanba, Juma.
    * Har bir katakchada dars nomini yozing.
    * Jadvalga `border`, `cellpadding`, `cellspacing` va `width` atributlarini qo'shing.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Dars jadvali</title>
    </head>
    <body>
      <h1>Dars jadvali</h1>
    
      <table border="1" cellpadding="10" cellspacing="0" width="80%">
        <tr>
          <th>Dars vaqti</th>
          <th>Dushanba</th>
          <th>Seshanba</th>
          <th>Chorshanba</th>
          <th>Payshanba</th>
          <th>Juma</th>
        </tr>
        <tr>
          <td>08:00 - 08:45</td>
          <td>Matematika</td>
          <td>Ona tili</td>
          <td>Ingliz tili</td>
          <td>Fizika</td>
          <td>Tarix</td>
        </tr>
        <tr>
          <td>08:50 - 09:35</td>
          <td>Fizika</td>
          <td>Adabiyot</td>
          <td>Kimyo</td>
          <td>Biologiya</td>
          <td>Geografiya</td>
        </tr>
        </table>
    
    </body>
    </html>
    ```

* **3-vazifa:  Anketa formasi**
    * HTML forma (`<form>`) yordamida anketa yarating.
    * Anketada quyidagi maydonlarni yarating:
        * Ism (`<input type="text">`). `placeholder` atributidan foydalanib, "Ismingizni kiriting" kabi ko'rsatma bering.
        * Familiya (`<input type="text">`).
        * Email (`<input type="email">`).
        * Telefon raqami (`<input type="tel">`).
        * Tug'ilgan kun (`<input type="date">`).
        * Jinsi (`<input type="radio">` tugmalari yordamida "Erkak" va "Ayol" variantlarini yarating).
        * Sevimli ranglar (`<input type="checkbox">` yordamida bir nechta ranglarni tanlash imkonini bering).
        * Qiziqishlar (`<textarea>`). `placeholder` atributidan foydalanib, "Qiziqishlaringizni yozing" kabi ko'rsatma bering.
    * Formada "Yuborish" tugmasi (`<button type="submit">`) bo'lsin.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
      <meta charset="UTF-8">
      <title>Anketa</title>
    </head>
    <body>
      <h1>Anketa</h1>
    
      <form>
        <label for="ism">Ism:</label>
        <input type="text" id="ism" name="ism" placeholder="Ismingizni kiriting"><br><br>
    
        <label for="familiya">Familiya:</label>
        <input type="text" id="familiya" name="familiya"><br><br>
    
        <button type="submit">Yuborish</button>
      </form>
    
    </body>
    </html>
    ```
</details>


<details>
   <summary>Semantik teglar (Semantic Tags / Семантические теги)</summary>

**Semantik teglar (Semantic Tags / Семантические теги)**

Oldingi darslarda biz HTML ning asosiy teglarini o'rgandik. Endi esa semantik teglar haqida bilib olamiz. 

Semantik teglar HTML5 da kiritilgan bo'lib, veb-sahifaning tuzilishini yanada aniqroq va mazmunli qilish uchun ishlatiladi. Ular brauzerga va qidiruv tizimlariga sahifaning turli qismlarining maqsadini tushunishga yordam beradi. Bu esa sahifaning SEO (Search Engine Optimization / Поисковая оптимизация) uchun ham foydali.

Ba'zi semantik teglar:

* `<header>`: Sahifaning sarlavha qismini belgilaydi. Odatda sayt nomi, logotipi, navigatsiya menyusi va boshqa kirish ma'lumotlarini o'z ichiga oladi.
* `<nav>`: Navigatsiya menyusini belgilaydi.
* `<main>`: Sahifaning asosiy mazmunini belgilaydi.
* `<article>`: Mustaqil tarkibni (masalan, blog posti, yangiliklar maqolasi) belgilaydi.
* `<aside>`: Asosiy mazmunga tegishli bo'lmagan yon tarkibni (masalan, yon panel, reklama) belgilaydi.
* `<footer>`: Sahifaning pastki qismini belgilaydi. Odatda mualliflik huquqi, aloqa ma'lumotlari va boshqa qo'shimcha ma'lumotlarni o'z ichiga oladi.

```html
<header>
  <h1>Veb-sayt sarlavhasi</h1>
  <nav>
    <ul>
      <li><a href="#">Bosh sahifa</a></li>
      <li><a href="#">Biz haqimizda</a></li>
      <li><a href="#">Aloqa</a></li>
    </ul>
  </nav>
</header>

<main>
  <article>
    <h2>Maqola sarlavhasi</h2>
    <p>Maqola matni...</p>
  </article>

  <aside>
    <h3>Yon panel</h3>
    <p>Qo'shimcha ma'lumot...</p>
  </aside>
</main>

<footer>
  <p>Mualliflik huquqi &copy; 2024</p>
</footer>
```

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifani bajaring:

* **Vazifa 10: Semantik teglar bilan veb-sahifani tuzing.**
    * `<header>`, `<nav>`, `<main>`, `<article>`, `<aside>` va `<footer>` teglaridan foydalanib, veb-sahifani tuzing.
    * Har bir tegga tegishli tarkibni joylashtiring.
    * Faylni saqlang va brauzerda yangilang. Veb-sahifaning tuzilishi semantik teglar yordamida aniqroq bo'lganini ko'rishingiz kerak.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mening birinchi veb-sahifam</title>
    </head>
    <body>
        <header>
          <h1>Saytimga xush kelibsiz!</h1>
          <nav>
            <ul>
              <li><a href="#">Bosh sahifa</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Aloqa</a></li>
            </ul>
          </nav>
        </header>
        
        <main>
          <article>
            <h2>Mening birinchi maqolam</h2>
            <p>Bu mening birinchi blog postim.</p>
          </article>
        
          <aside>
            <h3>So'nggi yangiliklar</h3>
            <p>Tez kunda yangi maqolalar!</p>
          </aside>
        </main>
        
        <footer>
          <p>Mualliflik huquqi &copy; 2024</p>
        </footer>
    </body>
    </html>
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  Shaxsiy veb-saytni semantik teglar bilan yaxshilang**
    * Oldingi darslarda yaratgan "Men haqimda" sahifasini semantik teglar yordamida yaxshilang.
    * Sahifada `<header>`, `<nav>`, `<main>` va `<footer>` teglaridan foydalaning.
    * Navigatsiya menyusida (`<nav>`) boshqa sahifalarga (masalan, "Bosh sahifa", "Blog", "Aloqa") havolalar qo'shing.
    * Asosiy ma'lumotni `<main>` tegi ichiga joylashtiring.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Men haqimda</title>
    </head>
    <body>
    
        <header>
            <h1>Men haqimda</h1>
            <nav>
            <ul>
                <li><a href="#">Bosh sahifa</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Aloqa</a></li>
            </ul>
            </nav>
        </header>
    
        <main>
            <img src="mening_rasmim.jpg" alt="Mening rasmim" width="200" height="300">
            <p>Mening ismim ... . Men ... yoshdaman.</p>
            <a href="https://sevimli_saytim.uz" title="Sevimli saytim">Sevimli saytimga tashrif buyuring</a>
        </main>
    
        <footer>
            <p>&copy; 2024 Mening saytim</p>
        </footer>
    
    </body>
    </html>
    ```

* **2-vazifa:  Blog postini semantik teglar bilan yarating**
    * Blog postiga o'xshash veb-sahifani yarating.
    * Sahifada `<header>`, `<nav>`, `<main>`, `<article>`, `<aside>` va `<footer>` teglaridan foydalaning.
    * Blog postingiz sarlavhasi uchun asosiy sarlavhadan (`<h1>`) foydalaning.
    * Blog posti mazmuni uchun bir nechta xatboshilar yozing.
    * Matnni sarlavhalar (`<h2>` yoki `<h3>`) yordamida bo'limlarga ajrating.
    * Blog postingizga tegishli rasm qo'shing.
    * Blog postingiz oxirida o'zingiz haqingizda qisqacha ma'lumot va ijtimoiy tarmoqlaringizga havolalarni qo'shing.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Blog Post</title>
    </head>
    <body>
        <header>
            <h1>Mening blogim</h1>
            <nav>
            <ul>
                <li><a href="#">Bosh sahifa</a></li>
                <li><a href="#">Maqolalar</a></li>
                <li><a href="#">Aloqa</a></li>
            </ul>
            </nav>
        </header>
    
        <main>
            <article>
                <h2>Maqola sarlavhasi</h2>
                <p>Maqola matni...</p>
            </article>
        
            <aside>
                <h3>Muallif haqida</h3>
                <p>Qo'shimcha ma'lumot...</p>
            </aside>
        </main>
    
        <footer>
            <p>Mualliflik huquqi &copy; 2024</p>
        </footer>
    
    </body>
    </html>
    ```

* **3-vazifa:  Mahsulot sahifasini semantik teglar bilan yarating**
    * Onlayn do'kon uchun mahsulot sahifasini yarating.
    * Sahifada `<header>`, `<nav>`, `<main>`, `<article>`, `<aside>` va `<footer>` teglaridan foydalaning.
    * Mahsulot nomini sarlavha (`<h1>`) sifatida yozing.
    * Mahsulot rasmini va tavsifini qo'shing.
    * Narxini va "Sotib olish" tugmasini qo'shing.
    * Yon panelda (`<aside>`) mahsulot haqida qo'shimcha ma'lumot yoki boshqa mahsulotlarni tavsiya qiling.

    ```html
    <!DOCTYPE html>
    <html lang="uz">
    <head>
        <meta charset="UTF-8">
        <title>Mahsulot</title>
    </head>
    <body>
        <header>
            <h1>Onlayn do'kon</h1>
            <nav>
            <ul>
                <li><a href="#">Bosh sahifa</a></li>
                <li><a href="#">Katalog</a></li>
                <li><a href="#">Aloqa</a></li>
            </ul>
            </nav>
        </header>
    
        <main>
            <article>
                <h1>Mahsulot nomi</h1>
                <img src="mahsulot.jpg" alt="Mahsulot">
                <p>Mahsulot tavsifi...</p>
                <p>Narxi: 10000 so'm</p>
                <button>Sotib olish</button>
            </article>
        
            <aside>
                <h3>Tavsiya etilgan mahsulotlar</h3>
                <ul>
                    <li>Mahsulot 1</li>
                    <li>Mahsulot 2</li>
                </ul>
            </aside>
        </main>
    
        <footer>
            <p>Mualliflik huquqi &copy; 2024</p>
        </footer>
    
    </body>
    </html>
    ```
</details>
<details>
<summary>JavaScript bilan interfaollik (1-qism)</summary>

#### Dars uchun qo'llanma

**JavaScript nima? (What is JavaScript? / Что такое JavaScript?)**

JavaScript veb-sahifalarga interfaollik va dinamik xatti-harakatlarni qo'shish uchun ishlatiladigan dasturlash tilidir. JavaScript yordamida siz foydalanuvchi harakatlariga javob berishingiz, ma'lumotlarni qayta ishlashingiz, veb-sahifaning mazmunini o'zgartirishingiz va boshqa ko'p narsalarni qilishingiz mumkin.

**JavaScript-ni HTML ga ulash (Linking JavaScript to HTML / Подключение JavaScript к HTML)**

JavaScript kodini HTML ga ulashning ikkita asosiy usuli mavjud:

1. **Tashqi fayl (External File / Внешний файл):** JavaScript kodini alohida `.js` fayliga yozasiz va uni `<script>` tegi yordamida HTML hujjatiga ulaysiz.

   ```html
   <script src="script.js"></script>
   ```

2. **Ichki skript (Internal Script / Внутренний скрипт):** JavaScript kodini `<script>` teglari ichida, HTML hujjatining istalgan joyiga yozishingiz mumkin.

   ```html
   <script>
       // JavaScript kodi bu yerda
   </script>
   ```

Odatda, JavaScript kodini `<body>` tegining oxirida ulash tavsiya etiladi, chunki bu sahifaning tezroq yuklanishiga yordam beradi.

**JavaScript asoslari (JavaScript Basics / Основы JavaScript)**

* **O'zgaruvchilar (Variables / Переменные):** Ma'lumotlarni saqlash uchun ishlatiladi. O'zgaruvchilarni e'lon qilish uchun `var`, `let` yoki `const` kalit so'zlaridan foydalaniladi.

   ```javascript
   let ism = "Ali";
   let yosh = 20;
   ```

* **Ma'lumotlar turlari (Data Types / Типы данных):** JavaScript da turli xil ma'lumotlar turlari mavjud, masalan:
    * `Number`: Raqamlar (masalan, `10`, `3.14`).
    * `String`: Matn (masalan, `"Salom"`, `'Dunyo'`).
    * `Boolean`: Mantiqiy qiymatlar (`true` yoki `false`).

* **Operatorlar (Operators / Операторы):** Ma'lumotlar ustida amallar bajarish uchun ishlatiladi. Ba'zi operatorlar:
    * Arifmetik operatorlar: `+`, `-`, `*`, `/`, `%`.
    * Taqqoslash operatorlari: `==`, `===`, `!=`, `>`, `<`, `>=`, `<=`.
    * Qo'shish operatori (`+`): Matnlarni birlashtirish uchun ham ishlatilishi mumkin.

* **Konsol (Console / Консоль):** Brauzerda JavaScript kodini ishga tushirish va natijalarni ko'rish uchun ishlatiladi. `console.log()` funksiyasi yordamida konsolga ma'lumotlarni chiqarish mumkin.


**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 4: JavaScript faylini yarating va uni HTML ga ulang.**
    * `script.js` nomli yangi fayl yarating.
    * Ushbu faylga oddiy JavaScript kodi yozing. Masalan, `console.log("Salom, JavaScript!");`
    * HTML faylingizda `<script>` tegini ishlatib, `script.js` faylini ulang.
    * Fayllarni saqlang va brauzerda oching. Brauzerning konsolida "Salom, JavaScript!" xabarini ko'rishingiz kerak.

* **Vazifa 5: O'zgaruvchilar bilan ishlang.**
    * JavaScript faylingizda turli xil ma'lumot turlari (`Number`, `String`, `Boolean`) uchun o'zgaruvchilar yarating.
    * O'zgaruvchilarga turli xil qiymatlar bering va ularni konsolga chiqaring.
    * `typeof` operatori yordamida o'zgaruvchilarning turini aniqlang va konsolga chiqaring.

* **Vazifa 6: Operatorlar bilan ishlang.**
    * Foydalanuvchidan ikkita sonni so'rang.
    * Bu sonlar ustida qo'shish, ayirish, ko'paytirish va bo'lish amallarini bajaring.
    * Natijalarni konsolga chiqaring.
    * Foydalanuvchidan ismini so'rang va uni "Salom, [ism]!" shaklida konsolga chiqaring.

* **Vazifa 7: Taqqoslash operatorlari bilan ishlang.**
    * Foydalanuvchidan ikkita sonni so'rang.
    * Bu sonlarni taqqoslang (`>`, `<`, `>=`, `<=`, `==`) va natijalarni konsolga chiqaring.
    * Masalan, "Birinchi son ikkinchi sondan katta", "Ikkala son teng" kabi xabarlarni chiqaring.

    ```javascript
    let son1 = prompt("Birinchi sonni kiriting:");
    let son2 = prompt("Ikkinchi sonni kiriting:");
    
    son1 = Number(son1);
    son2 = Number(son2);
    
    if (son1 > son2) {
      console.log("Birinchi son ikkinchi sondan katta");
    } else if (son1 < son2) {
      console.log("Birinchi son ikkinchi sondan kichik");
    } else {
      console.log("Ikkala son teng");
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  "O'zgaruvchilar va ma'lumotlar turlari"**
    * Turli xil ma'lumotlar turlari (`Number`, `String`, `Boolean`) uchun o'zgaruvchilar yarating.
    * O'zgaruvchilarga turli xil qiymatlar bering va ularni konsolga chiqaring.
    * `typeof` operatori yordamida o'zgaruvchilarning turini aniqlang va konsolga chiqaring.
    * O'zgaruvchilarning qiymatlarini o'zgartirib ko'ring va natijalarni konsolga chiqaring.


* **2-vazifa:  "Matematik amallar"**
    * Foydalanuvchidan uchta sonni so'rang.
    * Bu sonlarning o'rta arifmetigini hisoblang.
    * Natijani konsolga chiqaring.


* **3-vazifa:  "Eng katta son"**
    * Foydalanuvchidan uchta sonni so'rang.
    * Bu sonlarning eng kattasini toping va konsolga chiqaring.

</details>


<details>
<summary>JavaScript bilan interfaollik (2-qism)</summary>

#### Dars uchun qo'llanma

**Shartli operatorlar (Conditional Statements / Условные операторы)**

Shartli operatorlar kod bajarilishini boshqarish uchun ishlatiladi. Agar ma'lum bir shart bajarilsa, kodning bir qismi bajariladi, aks holda boshqa qismi bajariladi.

JavaScript da quyidagi shartli operatorlar mavjud:

* `if`: Agar shart bajarilsa, kod blokini bajaradi.
* `else`: Agar `if` sharti bajarilmasa, kod blokini bajaradi.
* `else if`: Agar `if` sharti bajarilmasa va boshqa bir shart bajarilsa, kod blokini bajaradi.

```javascript
if (shart) {
  // Kod bu yerda bajariladi, agar shart true bo'lsa
} else {
  // Kod bu yerda bajariladi, agar shart false bo'lsa
}
```

Masalan, quyidagi kod foydalanuvchining yoshini tekshiradi va agar u 18 dan katta bo'lsa, "Siz saylovda qatnashishingiz mumkin" xabarini konsolga chiqaradi:

```javascript
let yosh = prompt("Yoshingizni kiriting:");

if (yosh >= 18) {
  console.log("Siz saylovda qatnashishingiz mumkin");
} else {
  console.log("Siz saylovda qatnasha olmaysiz");
}
```

**Sikllar (Loops / Циклы)**

Sikllar kodning bir qismini bir necha marta takrorlash uchun ishlatiladi. JavaScript da quyidagi sikllar mavjud:

* `for`: Belgilangan marta takrorlanadigan sikl.
* `while`: Shart bajarilguncha takrorlanadigan sikl.

```javascript
for (let i = 0; i < 10; i++) {
  // Kod bu yerda 10 marta takrorlanadi
}

let i = 0;
while (i < 10) {
  // Kod bu yerda i 10 dan kichik bo'lguncha takrorlanadi
  i++;
}
```

Masalan, quyidagi kod 1 dan 10 gacha bo'lgan sonlarni konsolga chiqaradi:

```javascript
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 8:  "Juft yoki toq"**
    * Foydalanuvchidan sonni so'rang.
    * `if` operatori yordamida sonning juft yoki toqligini aniqlang.
    * Natijani konsolga chiqaring.

    ```javascript
    let son = Number(prompt("Son kiriting:"));
    
    if (son % 2 == 0) {
      console.log("Son juft");
    } else {
      console.log("Son toq");
    }
    ```

* **Vazifa 9:  "Baho"**
    * Foydalanuvchidan imtihon natijasini (0 dan 100 gacha) so'rang.
    * `if`, `else if` va `else` operatorlaridan foydalanib, baho qo'ying:
        * 90 dan 100 gacha: "A'lo"
        * 80 dan 89 gacha: "Yaxshi"
        * 70 dan 79 gacha: "Qoniqarli"
        * 60 dan 69 gacha: "O'rta"
        * 60 dan past: "Yomon"
    * Bahoni konsolga chiqaring.

    ```javascript
    let natija = Number(prompt("Imtihon natijasini kiriting (0-100):"));
    
    if (natija >= 90) {
      console.log("A'lo");
    } else if (natija >= 80) {
      console.log("Yaxshi");
    } else if (natija >= 70) {
      console.log("Qoniqarli");
    } else if (natija >= 60) {
      console.log("O'rta");
    } else {
      console.log("Yomon");
    }
    ```

* **Vazifa 10:  "1 dan 10 gacha bo'lgan sonlar"**
    * `for` sikli yordamida 1 dan 10 gacha bo'lgan sonlarni konsolga chiqaring.

    ```javascript
    for (let i = 1; i <= 10; i++) {
      console.log(i);
    }
    ```


**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

**(O'rta darajadagi vazifalar)**

* **1-vazifa:  "Musbat yoki manfiy"**
    * Foydalanuvchidan sonni so'rang.
    * `if` operatori yordamida sonning musbat, manfiy yoki nolga teng ekanligini aniqlang.
    * Natijani konsolga chiqaring.


* **2-vazifa:  "Eng katta son"**
    * Foydalanuvchidan ikkita sonni so'rang.
    * `if` operatori yordamida qaysi son kattaroq ekanligini aniqlang.
    * Natijani konsolga chiqaring.


* **3-vazifa:  "Kvadratning yuzasi"**
    * Foydalanuvchidan kvadratning tomonini so'rang.
    * Kvadratning yuzini hisoblang.
    * Natijani konsolga chiqaring.

* **4-vazifa:  "1 dan N gacha bo'lgan sonlar yig'indisi"**
    * Foydalanuvchidan sonni so'rang (`N`).
    * `for` sikli yordamida 1 dan `N` gacha bo'lgan sonlarning yig'indisini hisoblang.
    * Natijani konsolga chiqaring.


* **5-vazifa:  "Juft sonlar"**
    * `for` sikli yordamida 1 dan 50 gacha bo'lgan juft sonlarni konsolga chiqaring.


**(Murakkabroq vazifalar)**

* **6-vazifa:  "Yulduzcha chizish"**
    * Foydalanuvchidan sonni so'rang.
    * `for` sikli yordamida shu son qatoridan iborat yulduzcha shaklini konsolga chiqaring. Masalan, agar foydalanuvchi 5 kiritsa, quyidagi shakl chiqishi kerak:

    ```
    *
    **
    ***
    ****
    *****
    ```


* **7-vazifa:  "Sonni topish"**
    * 1 dan 100 gacha tasodifiy son o'ylang.
    * `while` sikli yordamida foydalanuvchidan sonni topishni so'rang.
    * Foydalanuvchi to'g'ri topmaguncha siklni takrorlang.
    * Foydalanuvchi to'g'ri topgandan so'ng, "Tabriklaymiz, siz to'g'ri topdingiz!" xabarini va foydalanuvchi necha marta urinib ko'rganini konsolga chiqaring.

</details>



<details>
<summary>JavaScript bilan interfaollik (3-qism)</summary>

#### Dars uchun qo'llanma

**Funksiyalar (Functions / Функции)**

Funksiyalar - bu ma'lum bir vazifani bajarish uchun mo'ljallangan qayta ishlatiladigan kod bloklari. Funksiyalar kodni tashkil qilish, takrorlanishni kamaytirish va kodni o'qishni osonlashtirish uchun ishlatiladi.

Funksiyani e'lon qilish uchun `function` kalit so'zidan foydalaniladi. Funksiya nomi, parametrlari va kod bloki ko'rsatiladi.

```javascript
function funksiyaNomi(parametr1, parametr2, ...) {
  // Kod bloki
}
```

Masalan, quyidagi funksiya ikkita sonni qabul qiladi va ularning yig'indisini qaytaradi:

```javascript
function yigindi(a, b) {
  return a + b;
}
```

Funksiyani chaqirish uchun uning nomini va qavslar ichida argumentlarni ko'rsatish kerak.

```javascript
let natija = yigindi(5, 3); // natija o'zgaruvchisi 8 ga teng bo'ladi
```

**Funksiyalarning afzalliklari:**

* **Kodni qayta ishlatish:** Bir marta yozilgan funksiyani kodning turli joylarida qayta-qayta ishlatish mumkin.
* **Kodni tashkil qilish:** Funksiyalar yordamida kodni kichikroq, boshqarish oson bo'lgan bloklarga ajratish mumkin.
* **Kodni o'qishni osonlashtirish:** Funksiyalar kodni yanada tushunarli va o'qish oson qiladi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 13:  "Salomlashish funksiyasi"**
    * Foydalanuvchidan ismini so'raydigan va uni "Salom, [ism]!" shaklida konsolga chiqaradigan funksiya yarating.

    ```javascript
    function salomlash(ism) {
      console.log("Salom, " + ism + "!");
    }
    
    let ism = prompt("Ismingizni kiriting:");
    salomlash(ism);
    ```

* **Vazifa 14:  "To'rtburchak yuzasi"**
    * To'rtburchakning yuzini hisoblaydigan funksiya yarating.
    * Funksiya to'rtburchakning eni va bo'yini argument sifatida qabul qilsin.
    * Funksiya yuzani qaytarsin.
    * Foydalanuvchidan to'rtburchakning eni va bo'yini so'rang va funksiya yordamida yuzani hisoblang.
    * Natijani konsolga chiqaring.

    ```javascript
    function togriTortburchakYuzasi(en, boy) {
      let yuza = en * boy;
      return yuza;
    }
    
    let en = Number(prompt("To'rtburchakning enini kiriting:"));
    let boy = Number(prompt("To'rtburchakning bo'yini kiriting:"));
    
    let yuza = togriTortburchakYuzasi(en, boy);
    console.log("To'rtburchakning yuzasi: " + yuza);
    ```

* **Vazifa 15:  "Sonlarni solishtirish"**
    * Ikkita sonni qabul qiladigan va ularning qaysi biri kattaroq ekanligini aniqlaydigan funksiya yarating.
    * Agar sonlar teng bo'lsa, "Sonlar teng" degan xabarni qaytaring.

    ```javascript
    function kattasiniTop(son1, son2) {
      if (son1 > son2) {
        return son1 + " kattaroq";
      } else if (son2 > son1) {
        return son2 + " kattaroq";
      } else {
        return "Sonlar teng";
      }
    }
    
    let son1 = Number(prompt("Birinchi sonni kiriting:"));
    let son2 = Number(prompt("Ikkinchi sonni kiriting:"));
    
    let natija = kattasiniTop(son1, son2);
    console.log(natija);
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

**(O'rta darajadagi vazifalar)**

* **1-vazifa:  "To'liq ism"**
    * Ism va familiyani qabul qilib, to'liq ismni qaytaradigan funksiya yarating.


* **2-vazifa:  "Sonlar o'rtacha qiymati"**
    * Ikkita sonni qabul qilib, ularning o'rtacha qiymatini qaytaradigan funksiya yarating.


* **3-vazifa:  "Matn uzunligi"**
    * Matnni qabul qilib, uning uzunligini qaytaradigan funksiya yarating.


**(Murakkabroq vazifalar)**

* **4-vazifa:  "Tub son"**
    * Sonni qabul qilib, uning tub son yoki yo'qligini aniqlaydigan funksiya yarating.
    * Tub son - bu faqat 1 ga va o'ziga bo'linadigan natural son.


* **5-vazifa:  "Teskari son"**
    * Sonni qabul qilib, uni teskari tartibda qaytaradigan funksiya yarating.
    * Masalan, agar 123 soni kiritilsa, funksiya 321 ni qaytarishi kerak.


* **6-vazifa:  "So'zlarni sanash"**
    * Matnni qabul qilib, undagi so'zlar sonini qaytaradigan funksiya yarating.

</details>


<details>
<summary>JavaScript bilan interfaollik (4-qism)</summary>

#### Dars uchun qo'llanma

**DOM (Document Object Model / Объектная модель документа)**

DOM (Document Object Model / Объектная модель документа) - bu HTML hujjatining ob'ektga yo'naltirilgan modeli. DOM veb-sahifani daraxt shaklida tasvirlaydi, bu yerda har bir tugun (node / узел) HTML elementini, atributini yoki matnini ifodalaydi.

JavaScript DOM yordamida veb-sahifani dinamik ravishda o'zgartirish, elementlarni qo'shish, o'chirish yoki o'zgartirish, atributlarni o'rnatish, foydalanuvchi hodisalariga javob berish va boshqa ko'p narsalarni qilish imkonini beradi.

**DOM elementlarini tanlash (Selecting DOM Elements / Выбор элементов DOM)**

DOM elementlarini tanlash uchun quyidagi usullardan foydalanish mumkin:

* `getElementById()`: ID atributi bo'yicha elementni tanlaydi.
* `getElementsByTagName()`: Teg nomi bo'yicha elementlarni tanlaydi.
* `getElementsByClassName()`: Klass nomi bo'yicha elementlarni tanlaydi.
* `querySelector()`: CSS selektori yordamida birinchi elementni tanlaydi.
* `querySelectorAll()`: CSS selektori yordamida barcha elementlarni tanlaydi.

**DOM elementlarini o'zgartirish (Modifying DOM Elements / Изменение элементов DOM)**

DOM elementlarini o'zgartirish uchun quyidagi xossalar va metodlardan foydalanish mumkin:

* `innerHTML`: Elementning HTML mazmunini o'rnatadi yoki oladi.
* `textContent`: Elementning matn mazmunini o'rnatadi yoki oladi.
* `style`: Elementning CSS stillarini o'rnatadi.
* `setAttribute()`: Elementning atributini o'rnatadi.
* `getAttribute()`: Elementning atributini oladi.
* `appendChild()`: Elementga yangi bola elementini qo'shadi.
* `removeChild()`: Elementdan bola elementini o'chiradi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 16:  Elementni ID bo'yicha tanlang va uning mazmunini o'zgartiring.**
    * HTML faylingizda ID atributiga ega bo'lgan element yarating (masalan, `<p id="my-paragraph">`).
    * JavaScript faylingizda `getElementById()` metodi yordamida bu elementni tanlang.
    * `innerHTML` xossasi yordamida elementning mazmunini o'zgartiring.

    ```javascript
    let element = document.getElementById("my-paragraph");
    element.innerHTML = "Yangi matn";
    ```

* **Vazifa 17:  Elementlarni teg nomi bo'yicha tanlang va ularning stillarini o'zgartiring.**
    * HTML faylingizda bir nechta bir xil tegga ega bo'lgan elementlar yarating (masalan, bir nechta `<p>` teglari).
    * JavaScript faylingizda `getElementsByTagName()` metodi yordamida bu elementlarni tanlang.
    * Sikl yordamida har bir elementning stilini o'zgartiring (masalan, rangini yoki shriftini).

    ```javascript
    let paragraphs = document.getElementsByTagName("p");
    
    for (let i = 0; i < paragraphs.length; i++) {
      paragraphs[i].style.color = "red";
    }
    ```

* **Vazifa 18:  Elementga yangi atribut qo'shing.**
    * HTML faylingizda biror element yarating.
    * JavaScript faylingizda `setAttribute()` metodi yordamida bu elementga yangi atribut qo'shing (masalan, `title` atributi).

    ```javascript
    let link = document.querySelector("a");
    link.setAttribute("title", "Bu havola");
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

* **1-vazifa:  "Rasmni o'zgartirish"**
    * HTML faylingizda rasm (`<img>`) qo'shing.
    * JavaScript faylingizda tugma (`<button>`) yarating.
    * Tugma bosilganda, rasmning `src` atributi o'zgarsin va boshqa rasm ko'rsatilsin.


* **2-vazifa:  "Ro'yxatga element qo'shish"**
    * HTML faylingizda ro'yxat (`<ul>` yoki `<ol>`) yarating.
    * JavaScript faylingizda tugma (`<button>`) yarating.
    * Tugma bosilganda, ro'yxatga yangi element (`<li>`) qo'shilsin.


* **3-vazifa:  "Matnni yashirish va ko'rsatish"**
    * HTML faylingizda matn (`<p>`) va tugma (`<button>`) yarating.
    * JavaScript faylingizda tugma bosilganda matnni yashiradigan va ko'rsatadigan kod yozing.
    * Matnni yashirish uchun `style.display = "none";` xossasidan, ko'rsatish uchun esa `style.display = "block";` xossasidan foydalaning.

</details>


<details>
<summary>JavaScript bilan interfaollik (5-qism)</summary>

#### Dars uchun qo'llanma

**Hodisalar (Events / События)**

Hodisalar (events / события) - bu veb-sahifada yoki brauzerda sodir bo'ladigan harakatlar. Masalan, foydalanuvchi tugmani bosganda, sichqonchani harakatlantirganda, klaviaturada tugmani bosganda yoki sahifa yuklanganda hodisalar sodir bo'ladi.

JavaScript yordamida siz ushbu hodisalarga javob berishingiz va kodni bajarishingiz mumkin. Buning uchun **hodisalarni qayta ishlash** (event handling / обработка событий) dan foydalaniladi.

**Hodisalarni qayta ishlash (Event Handling / Обработка событий)**

Hodisalarni qayta ishlash uchun siz HTML elementlariga **hodisalarni tinglovchilar** (event listeners / обработчики событий) ni biriktirishingiz mumkin. Hodisa tinglovchisi - bu hodisa sodir bo'lganda bajariladigan funksiya.

Hodisa tinglovchisini biriktirishning ikkita asosiy usuli mavjud:

1. **HTML atributlari:** Hodisa nomini atribut sifatida HTML tegiga qo'shish va atribut qiymatiga JavaScript kodini yozish.

   ```html
   <button onclick="alert('Tugma bosildi!')">Bosish</button>
   ```

2. **`addEventListener()` metodi:** JavaScript da `addEventListener()` metodi yordamida hodisa tinglovchisini biriktirish.

   ```javascript
   let tugma = document.querySelector("button");

   tugma.addEventListener("click", function() {
     alert("Tugma bosildi!");
   });
   ```

`addEventListener()` metodi ikkita argument qabul qiladi:

* Hodisa nomi (masalan, `click`, `mouseover`, `keydown`).
* Hodisa sodir bo'lganda bajariladigan funksiya.

**Ba'zi umumiy hodisalar:**

* `click`: Element bosilganda sodir bo'ladi.
* `mouseover`: Sichqoncha elementi ustiga qo'yilganda sodir bo'ladi.
* `mouseout`: Sichqoncha elementdan olib tashlanganda sodir bo'ladi.
* `keydown`: Klaviaturada tugma bosilganda sodir bo'ladi.
* `keyup`: Klaviaturada tugma qo'yib yuborilganda sodir bo'ladi.
* `load`: Sahifa to'liq yuklanganda sodir bo'ladi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 19:  "Tugmani bosing"**
    * HTML faylingizda tugma (`<button>`) yarating.
    * JavaScript faylingizda `addEventListener()` metodi yordamida tugmaga `click` hodisasi tinglovchisini biriktiring.
    * Tugma bosilganda, konsolga "Tugma bosildi!" xabarini chiqaring.

    ```javascript
    let tugma = document.querySelector("button");
    
    tugma.addEventListener("click", function() {
      console.log("Tugma bosildi!");
    });
    ```

* **Vazifa 20:  "Rangni o'zgartirish"**
    * HTML faylingizda `<div>` elementi yarating.
    * JavaScript faylingizda `addEventListener()` metodi yordamida `<div>` elementiga `mouseover` va `mouseout` hodisalari tinglovchilarini biriktiring.
    * Sichqoncha elementi ustiga qo'yilganda, uning fon rangini qizilga o'zgartiring.
    * Sichqoncha elementdan olib tashlanganda, uning fon rangini asl holatiga qaytaring.

    ```javascript
    let div = document.querySelector("div");
    
    div.addEventListener("mouseover", function() {
      this.style.backgroundColor = "red";
    });
    
    div.addEventListener("mouseout", function() {
      this.style.backgroundColor = ""; // Asl rangga qaytarish
    });
    ```

* **Vazifa 21:  "Matnni yozish"**
    * HTML faylingizda matn maydoni (`<input type="text">`) yarating.
    * JavaScript faylingizda `addEventListener()` metodi yordamida matn maydoniga `keyup` hodisasi tinglovchisini biriktiring.
    * Foydalanuvchi matn maydoniga biror narsa yozganda, yozilgan matnni konsolga chiqaring.

    ```javascript
    let matnMaydoni = document.querySelector("input");
    
    matnMaydoni.addEventListener("keyup", function() {
      console.log(this.value);
    });
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

**(O'rta darajadagi vazifalar)**

* **1-vazifa:  "Tugmani sanash"**
    * HTML faylingizda tugma (`<button>`) va sonni ko'rsatadigan element (`<p>`) yarating.
    * JavaScript faylingizda o'zgaruvchi yarating va unga 0 qiymatini bering.
    * `addEventListener()` metodi yordamida tugmaga `click` hodisasi tinglovchisini biriktiring.
    * Tugma bosilganda, o'zgaruvchining qiymatini 1 ga oshiring va yangi qiymatni `<p>` elementida ko'rsating.

* **2-vazifa:  "Rasmni almashtirish"**
    * HTML faylingizda ikkita rasm (`<img>`) qo'shing, lekin faqat bittasini ko'rsating.
    * JavaScript faylingizda tugma (`<button>`) yarating.
    * Tugma bosilganda, ko'rinib turgan rasmni yashiring va ikkinchi rasmni ko'rsating.


* **3-vazifa:  "Matnni o'zgartirish"**
    * HTML faylingizda matn (`<p>`) va tugma (`<button>`) yarating.
    * JavaScript faylingizda tugma bosilganda matnni o'zgartiradigan kod yozing.
    * Masalan, "Salom, Dunyo!" matnini "Xayr, Dunyo!" ga o'zgartiring.


**(Murakkabroq vazifalar)**

* **4-vazifa:  "Sichqoncha koordinatalari"**
    * HTML faylingizda `<div>` elementi yarating.
    * JavaScript faylingizda `addEventListener()` metodi yordamida `<div>` elementiga `mousemove` hodisasi tinglovchisini biriktiring.
    * Sichqoncha elementi ustida harakatlanganda, sichqonchaning koordinatalarini (x va y) konsolga chiqaring.
    * Qo'shimcha: Sichqonchaning koordinatalarini `<div>` elementi ichida ham ko'rsating.


* **5-vazifa:  "Tugma bilan hisoblagich"**
    * HTML faylingizda ikkita tugma ("+" va "-") va sonni ko'rsatadigan element (`<p>`) yarating.
    * JavaScript faylingizda o'zgaruvchi yarating va unga 0 qiymatini bering.
    * `addEventListener()` metodi yordamida tugmalarga `click` hodisasi tinglovchilarini biriktiring.
    * "+" tugmasi bosilganda, o'zgaruvchining qiymatini 1 ga oshiring.
    * "-" tugmasi bosilganda, o'zgaruvchining qiymatini 1 ga kamaytiring.
    * O'zgaruvchining yangi qiymatini `<p>` elementida ko'rsating.


* **6-vazifa:  "Klaviatura hodisalari"**
    * HTML faylingizda matn maydoni (`<input type="text">`) yarating.
    * JavaScript faylingizda `addEventListener()` metodi yordamida matn maydoniga `keydown`, `keyup` va `keypress` hodisalari tinglovchilarini biriktiring.
    * Har bir hodisa sodir bo'lganda, konsolga quyidagi ma'lumotlarni chiqaring:
        * Hodisa nomi (masalan, "keydown").
        * Bosigan tugmaning kodi (`event.code`).
        * Bosigan tugmaning nomi (`event.key`).


</details>

<details>
<summary>JavaScript bilan interfaollik (5-qism)</summary>
#### Dars uchun qo'llanma

**Massivlar (Arrays / Массивы)**

Massivlar (arrays / массивы) - bu bir nechta qiymatlarni saqlash uchun ishlatiladigan maxsus ma'lumotlar tuzilmasi. Massivlar elementlarning tartiblangan to'plami bo'lib, har bir element indeks (index / индекс) yordamida aniqlanadi. Indekslar 0 dan boshlanadi.

Massivlarni yaratish uchun kvadrat qavslar (`[]`) ishlatiladi. Elementlar vergul (`,`) bilan ajratiladi.

```javascript
let mevalar = ["olma", "banan", "anor"];
let sonlar = [1, 2, 3, 4, 5];
let aralash = [1, "salom", true, null];
```

**Massiv elementlariga kirish (Accessing Array Elements / Доступ к элементам массива)**

Massiv elementlariga kirish uchun indeksdan foydalaniladi.

```javascript
console.log(mevalar[0]); // "olma" ni konsolga chiqaradi
console.log(sonlar[2]); // 3 ni konsolga chiqaradi
```

**Massivlar bilan ishlash (Working with Arrays / Работа с массивами)**

JavaScript da massivlar bilan ishlash uchun ko'plab metodlar mavjud. Ba'zi foydali metodlar:

* `push()`: Massiv oxiriga yangi element qo'shadi.
* `pop()`: Massiv oxiridan elementni o'chiradi.
* `shift()`: Massiv boshidan elementni o'chiradi.
* `unshift()`: Massiv boshiga yangi element qo'shadi.
* `length`: Massiv uzunligini (elementlar sonini) qaytaradi.
* `indexOf()`: Elementning massivda birinchi uchragan indeksini qaytaradi.
* `slice()`: Massivning bir qismini yangi massiv sifatida qaytaradi.
* `splice()`: Massivdan elementlarni qo'shadi yoki o'chiradi.
* `forEach()`: Massivning har bir elementi uchun funksiyani bajaradi.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 19:  Massiv yarating va elementlarini konsolga chiqaring.**
    * Sevimli ranglaringiz ro'yxatini saqlaydigan massiv yarating.
    * Massivning har bir elementini konsolga chiqaring.

    ```javascript
    let ranglar = ["qizil", "yashil", "ko'k"];
    
    for (let i = 0; i < ranglar.length; i++) {
      console.log(ranglar[i]);
    }
    ```

* **Vazifa 20:  Massivga elementlar qo'shing va o'chiring.**
    * Sonlarni saqlaydigan massiv yarating.
    * `push()` metodi yordamida massiv oxiriga yangi son qo'shing.
    * `unshift()` metodi yordamida massiv boshiga yangi son qo'shing.
    * `pop()` metodi yordamida massiv oxiridan sonni o'chiring.
    * `shift()` metodi yordamida massiv boshidan sonni o'chiring.
    * Har bir o'zgarishdan keyin massivni konsolga chiqaring.

    ```javascript
    let sonlar = [1, 2, 3];
    
    sonlar.push(4); // [1, 2, 3, 4]
    console.log(sonlar);
    
    sonlar.unshift(0); // [0, 1, 2, 3, 4]
    console.log(sonlar);
    
    sonlar.pop(); // [0, 1, 2, 3]
    console.log(sonlar);
    
    sonlar.shift(); // [1, 2, 3]
    console.log(sonlar);
    ```

* **Vazifa 21:  Massiv elementlarini toping.**
    * Ismlarni saqlaydigan massiv yarating.
    * `indexOf()` metodi yordamida ma'lum bir ismning massivda bor-yo'qligini tekshiring.
    * Agar ism massivda bo'lsa, uning indeksini konsolga chiqaring.
    * Agar ism massivda bo'lmasa, "-1" ni konsolga chiqaring.

    ```javascript
    let ismlar = ["Ali", "Vali", "Olim"];
    
    let index = ismlar.indexOf("Vali");
    console.log(index); // 1
    
    index = ismlar.indexOf("Hasan");
    console.log(index); // -1
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

**(O'rta darajadagi vazifalar)**

* **1-vazifa:  "Eng katta son"**
    * Sonlar massivini yarating.
    * Massivdagi eng katta sonni toping va konsolga chiqaring.


* **2-vazifa:  "O'rtacha qiymat"**
    * Sonlar massivini yarating.
    * Massivdagi sonlarning o'rtacha qiymatini hisoblang va konsolga chiqaring.


* **3-vazifa:  "Teskari massiv"**
    * Matnlar massivini yarating.
    * Massivni teskari tartibda konsolga chiqaring.


**(Murakkabroq vazifalar)**

* **4-vazifa:  "Takrorlanishlarni olib tashlash"**
    * Massivda takrorlanadigan elementlarni olib tashlang.
    * Masalan, `[1, 2, 2, 3, 4, 4, 5]` massivini `[1, 2, 3, 4, 5]` ga o'zgartiring.


* **5-vazifa:  "Massivni saralash"**
    * Sonlar massivini o'sish tartibida saralang.


* **6-vazifa:  "Ikki o'lchamli massiv"**
    * Ikki o'lchamli massiv yarating (massivlar massivi).
    * Massiv elementlarini konsolga chiqaring.


</details>



<details>
<summary>JavaScript bilan interfaollik (6-qism)</summary>

#### Dars uchun qo'llanma

**Obyektlar (Objects / Объекты)**

Obyektlar (objects / объекты) - bu JavaScript-da murakkab ma'lumotlar tuzilmasi. Ular xossalar (properties / свойства) va metodlar (methods / методы) dan iborat. Xossalar obyektning xususiyatlarini saqlaydi, metodlar esa obyekt ustida amallar bajarish uchun ishlatiladi.

Obyektlarni yaratish uchun jingalak qavslar (`{}`) ishlatiladi. Xossalar va metodlar vergul (`,`) bilan ajratiladi.

```javascript
let talaba = {
  ism: "Ali",
  familiya: "Valiyev",
  yosh: 20,
  salomlash: function() {
    console.log("Salom, mening ismim " + this.ism + "!");
  }
};
```

Bu misolda `talaba` obyekti `ism`, `familiya` va `yosh` xossalariga, shuningdek, `salomlash` metodiga ega.

**Obyekt xossalariga kirish (Accessing Object Properties / Доступ к свойствам объекта)**

Obyekt xossalariga kirish uchun nuqta (`.`) yoki kvadrat qavslar (`[]`) ishlatiladi.

```javascript
console.log(talaba.ism); // "Ali" ni konsolga chiqaradi
console.log(talaba["familiya"]); // "Valiyev" ni konsolga chiqaradi
```

**Obyekt metodlarini chaqirish (Calling Object Methods / Вызов методов объекта)**

Obyekt metodlarini chaqirish uchun nuqta (`.`) va qavslar (`()`) ishlatiladi.

```javascript
talaba.salomlash(); // "Salom, mening ismim Ali!" ni konsolga chiqaradi
```

**`this` kalit so'zi**

`this` kalit so'zi obyektning o'ziga ishora qiladi. Obyekt metodi ichida `this` yordamida obyektning xossalariga va boshqa metodlariga kirish mumkin.

**Amaliy mashg'ulotlar**

Endi o'qituvchingiz bilan birgalikda quyidagi vazifalarni bajaring:

* **Vazifa 22:  Obyekt yarating va uning xossalarini konsolga chiqaring.**
    * O'zingiz haqingizdagi ma'lumotlarni saqlaydigan obyekt yarating (ism, familiya, yosh, sevimli rang va hokazo).
    * Obyektning barcha xossalarini konsolga chiqaring.

    ```javascript
    let shaxs = {
      ism: "Nodira",
      familiya: "Siddiqova",
      yosh: 18,
      sevimliRang: "ko'k"
    };
    
    console.log(shaxs.ism);
    console.log(shaxs.familiya);
    console.log(shaxs.yosh);
    console.log(shaxs.sevimliRang);
    ```

* **Vazifa 23:  Obyektga metod qo'shing.**
    * Yuqorida yaratgan obyektga `toliqIsm()` nomli metod qo'shing.
    * Bu metod shaxsning to'liq ismini (ism va familiya) qaytarsin.
    * Metodni chaqirib, natijani konsolga chiqaring.

    ```javascript
    shaxs.toliqIsm = function() {
      return this.ism + " " + this.familiya;
    };
    
    console.log(shaxs.toliqIsm());
    ```

* **Vazifa 24:  Obyektlar massivi**
    * Talabalar haqidagi ma'lumotlarni saqlaydigan obyektlar massivini yarating.
    * Har bir obyektda talabaning ismi, familiyasi va yoshi bo'lsin.
    * Massivning har bir elementi (obyekti) uchun talabaning to'liq ismini va yoshini konsolga chiqaring.

    ```javascript
    let talabalar = [
      { ism: "Ali", familiya: "Valiyev", yosh: 20 },
      { ism: "Vali", familiya: "Aliyev", yosh: 21 },
      { ism: "Olim", familiya: "Hakimov", yosh: 19 }
    ];
    
    for (let i = 0; i < talabalar.length; i++) {
      let talaba = talabalar[i];
      console.log(talaba.ism + " " + talaba.familiya + ", " + talaba.yosh + " yoshda");
    }
    ```

**Mustaqil mashqlar**

O'rganganlaringizni mustahkamlash uchun quyidagi vazifalarni mustaqil bajarib ko'ring:

**(O'rta darajadagi vazifalar)**

* **1-vazifa:  "Kitob obyekti"**
    * Kitob haqidagi ma'lumotlarni saqlaydigan obyekt yarating (nomi, muallifi, nashr yili, janri).
    * Obyektning barcha xossalarini konsolga chiqaring.


* **2-vazifa:  "Hayvon obyekti"**
    * Hayvon haqidagi ma'lumotlarni saqlaydigan obyekt yarating (turi, nomi, yoshi, rangi).
    * Obyektga `ovozChiqar()` nomli metod qo'shing.
    * Bu metod hayvonning ovozini konsolga chiqarsin (masalan, "miyov" yoki "vov").


**(Murakkabroq vazifalar)**

* **3-vazifa:  "Talabalar ro'yxati"**
    * Talabalar haqidagi ma'lumotlarni saqlaydigan obyektlar massivini yarating.
    * Har bir obyektda talabaning ismi, familiyasi, yoshi va baholari massivi bo'lsin.
    * Har bir talaba uchun uning o'rtacha bahosini hisoblang va konsolga chiqaring.


* **4-vazifa:  "Mahsulotlar katalogi"**
    * Mahsulotlar haqidagi ma'lumotlarni saqlaydigan obyektlar massivini yarating.
    * Har bir obyektda mahsulotning nomi, narxi, tavsifi va rasmi bo'lsin.
    * Ushbu ma'lumotlarni HTML da jadval ko'rinishida chiqaring.
    * JavaScript yordamida mahsulotlarni narx bo'yicha saralang.

</details>
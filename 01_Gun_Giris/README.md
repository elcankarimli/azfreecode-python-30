

# 📘 Gün 1: Giriş və Python

> **Təbriklər!** Sən artıq **30 Gündə Python** proqramlaşdırma marafonuna başlamaq qərarına gəldin. Bu marafonun sonunda sən bir Python proqramçısı olmaq üçün lazım olan bütün əsas anlayışları mənimsəyəcək və kursun sonunda **AzFreeCode** sertifikatını qazanacaqsan.

---

## 🌟 Python Nədir və Sənayedə Harada İstifadə Olunur?

Python, sadəliyi və istifadə asanlığı ilə tanınan ümumi təyinatlı proqramlaşdırma dilidir. Məhz bu asanlıq Python-u müasir dövrün ən populyar dilinə çevirmişdir. Python məlumat elmindən süni intellektə, veb inkişafından avtomatlaşdırmaya qədər bir çox sahədə tətbiq olunur.



### 📊 1. Məlumat Elmi və Süni İntellekt (AI)
Python hazırda əksər məlumat alimləri (data scientists) və maşın öyrənməsi mühəndislərinin istifadə etdiyi əsas dildir. `Pandas` və `Numpy` kimi kitabxanalar məlumat analizini asanlaşdırır, `Tensorflow` və `Scikit-learn` isə maşın öyrənməsi və AI modelləri ilə işləməyi hər kəs üçün əlçatan edir.

### 🌐 2. Veb İnkişafı
Veb inkişafında Python-un `Django`, `FastAPI` və `Flask` kimi çərçivələri (frameworks) tərtibatçılara minimum səylə genişləndirilə bilən və təhlükəsiz back-end sistemləri qurmağa imkan verir. **Instagram** və **Pinterest** kimi bir çox sosial media platformaları öz back-end sistemlərində Python-dan istifadə edirlər.

### 🛡️ 3. Kibertəhlükəsizlik
Kibertəhlükəsizlik mütəxəssisləri və etik hakerlər zərərli proqramları (malware) və virusları aşkar etmək, avtomatlaşdırılmış təhlükəsizlik skanları yaratmaq və təhdidləri analiz etmək üçün Python-dan istifadə edirlər.

### 🤖 4. IoT və Quraşdırılmış Sistemlər
Python `Raspberry Pi` və `MicroPython` uyğun gələn lövhələr kimi mikrokompüterlərdə yaxşı işləyir. Bu da sizə ağıllı ev cihazları, hava monitorinq stansiyaları və s. kimi hər növ IoT layihələri qurmağa imkan verir.

### ⚙️ 5. DevOps və Proqram Testi
Python DevOps sahəsində CI/CD skriptlərinin yazılması və infrastrukturun idarə edilməsi üçün geniş istifadə olunur. Proqram təminatının sınaqdan keçirilməsində (testing) `pytest` kimi alətlər etibarlı test dəstləri yaratmağa kömək edir. Sistem administratorları isə server monitorinqi və loqların idarə edilməsi üçün Python-a güvənirlər.

### 🚀 6. Avtomatlaşdırma (Automation)
Python-un ən böyük güclərindən biri avtomatlaşdırmadır. Elektron cədvəllərdən məlumat çıxarmaq, e-poçt göndərmək və yerli fayllarla işləmək kimi təkrarlanan tapşırıqlar üçün sadə skriptlər yaza bilərsiniz. `Selenium` və `BeautifulSoup` kimi kitabxanalar veb-saytlarla qarşılıqlı əlaqəni asanlaşdırır, beləliklə siz ictimai məlumatları toplaya (scraping) və bulud yerləşdirmələrini idarə edə bilərsiniz.

---

## 🛠️ İş Mühitinin Qurulması

### 1️⃣ Python-un Quraşdırılması
Python skriptlərini işlətmək üçün əvvəlcə onu [python.org](https://www.python.org/) saytından yükləməlisiniz.
* **Vacib:** Yükləmə zamanı **"Add Python to PATH"** xanasını mütləq işarələyin.
* **Yoxlama:** Terminalda `python3 --version` yazaraq quraşdırılmanı yoxlayın.

### 2️⃣ Python Shell (İnteraktiv Qabıq)
Python interpretasiya olunan dildir, yəni kodu sətir-sətir icra edir. Terminalda `python` yazaraq Python Shell-i aça bilərsiniz.

### 3️⃣ Visual Studio Code (VS Code)
Böyük layihələr üçün biz **Visual Studio Code** redaktorundan istifadə edəcəyik.
* [Buradan yükləyin](https://code.visualstudio.com/)
* İlk faylınızı yaradın: `helloworld.py`.

---

## 🏗️ Python-un Əsasları

* **Sintaksis və Abzaslar:** Python kod bloklarını yaratmaq üçün boşluqlardan (indentation) istifadə edir.
* **Şərhlər:** `#` simvolu ilə başlayan sətirlər Python tərəfindən icra olunmur.

---

## 📋 Məlumat Tipləri (Data Types)

| Tip | Nümunə | Təsvir |
| :--- | :--- | :--- |
| **Number** | `10`, `3.14` | Tam və onluq ədədlər |
| **String** | `"AzFreeCode"` | Mətn məlumatları |
| **Booleans** | `True`, `False` | Məntiqi dəyərlər |
| **List** | `[1, 2, 3]` | Dəyişdirilə bilən siyahı |
| **Dictionary** | `{'key': 'value'}` | Açar-dəyər cütlüyü |

---

## 💻 1-ci Günün Tapşırıqları

### Səviyyə 1
1. Python versiyanı yoxla.
2. Python Shell-də 3 və 4 rəqəmləri ilə riyazi əməlləri yerinə yetir.
3. Öz adını, soyadını və "I am enjoying 30 days of python" cümləsini çap et.
4. `type()` funksiyası ilə `10`, `9.8`, `['Asabeneh', 'Python']` tiplərini yoxla.

### Səviyyə 2
1. `day_1` qovluğunda `helloworld.py` faylı yarat və yuxarıdakı tapşırıqları orada `print()` ilə təkrarla.

### Səviyyə 3
1. Hər bir məlumat tipinə aid öz nümunəni yaz.
2. (2, 3) və (10, 8) nöqtələri arasındakı **Evklid məsafəsini** hesablayan kod yaz.

Təbriklər! 1-ci günü uğurla tamamladın! 🎉
---
<p align="center">🧡 <b>Happy Coding!</b> 🧡</p>

---
<p align="center">🧡 <b>AzFreeCode - Gələcəyi kodla! </b> 🧡</p>


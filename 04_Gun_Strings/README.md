---

# 📅 Gün 04: Stringlər (Mətnlər)

Proqramlaşdırmada hər hansı bir mətn məlumatı **String** adlanır. Python-da dırnaq işarəsi (`'`, `"`, və ya `"""`) daxilində yazılan hər şey stringdir.

---

## 🏗️ 1. String Yaradılması və Çoxsətirli Mətnlər
Stringləri tək, cüt və ya üçlü dırnaqla yarada bilərik.

*   **Tək/Cüt dırnaq:** Qısa, tək sətirlik mətnlər üçün.
*   **Üçlü dırnaq (`"""`):** Çoxsətirli mətnlər (məsələn, bir sənəd və ya kitab abzası) üçün istifadə olunur.

```python
name = 'Elcan'
status = "Python öyrənir"
multiline = """Bu layihə AzFreeCode tərəfindən
təşkil olunmuş 30 günlük
Python marafonudur."""
```

---

## 🔗 2. String Birləşdirmə (Concatenation)
İki və ya daha çox mətni `+` operatoru ilə birləşdirə bilərik.
*   `full_name = "Elcan" + " " + "Kərimli"`

---

## 🛠️ 3. String Metodları (Ən Vacibləri)
Python-da mətnlər üzərində işləmək üçün hazır "alətlər" var:

| Metod | Funksiyası | Nümunə |
| :--- | :--- | :--- |
| `upper()` | Hamısını BÖYÜK hərf edir | `"python".upper()` -> `PYTHON` |
| `lower()` | Hamısını kiçik hərf edir | `"ELCAN".lower()` -> `elcan` |
| `capitalize()` | Yalnız ilk hərfi böyüdür | `"azFreeCode".capitalize()` -> `Azfreecode` |
| `strip()` | Başdakı və sondakı boşluqları silir | `"  salam  ".strip()` -> `salam` |
| `split()` | Mətni hissələrə bölür (list yaradır) | `"A, B, C".split(",")` -> `['A', ' B', ' C']` |
| `replace()` | Bir hissəni başqası ilə dəyişir | `"Hi".replace("Hi", "Salam")` -> `Salam` |

---

## 🎯 4. İndeksləmə və Slicing (Kəsmə)
Mətnin hər bir hərfinin bir "ünvanı" (indeksi) var. **Sayma həmişə 0-dan başlayır!**



*   **Müsbət indeks:** Soldan sağa (0, 1, 2...).
*   **Mənfi indeks:** Sağdan sola (-1, -2...).
*   **Slicing:** `string[start:stop:step]` formatında mətndən parça qoparmaq olar.
    *   `"Python"[:2]` -> `Py` (0 və 1-ci indeks).
    *   `"Python"[::-1]` -> `nohtyP` (Mətni tərsinə çevirir).

---

## 🖋️ 5. String Formatting (Yeni Üsul: f-strings)
Dəyişənləri mətnin içinə yerləşdirməyin ən sürətli və rahat yolu **f-strings** üsuludur.

```python
radius = 10
area = 3.14 * radius ** 2
# f-string istifadəsi
print(f"Radiusu {radius} olan dairənin sahəsi: {area}")
```

---

## 💻 Gün 04 - Praktik Tapşırıqlar (Laboratoriya)

1.  `'Coding', 'For' , 'All'` sözlərini birləşdirərək bir dəyişənə mənimsət və uzunluğunu tap.
2.  Həmin dəyişəni tamamilə böyük hərflərə çevir.
3.  "Coding For All" mətnindən ilk sözü (Coding) `slice` vasitəsilə kəsib çıxart.
4.  Aşağıdakı cümlədə "because" sözünün ilk harda işləndiyini tap:
    *"You cannot end a sentence with because because because is a conjunction"*.
5.  `'   Coding For All      '` mətninin əvvəlindəki və sonundakı boşluqları təmizlə.

---

### 🛡️ Kiber-Təhlükəsizlik Notu:
Stringlər sadəcə mətn deyil. Kiber-təhlükəsizlikdə **OSINT** edərkən və ya log fayllarını analiz edərkən `split()`, `find()` və `strip()` metodları sənin ən yaxın dostun olacaq. Məsələn, bir IP ünvanını `.` işarəsinə görə parçalayıb analiz etmək üçün bu metodlar şərtdir!"

---
**Uğurlar! AzFreeCode ilə irəliyə!** 🚀

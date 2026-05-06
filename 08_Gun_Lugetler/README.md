
---

# 📘Gün 08 — Dictionaries (Lüğətlər)
### "Məlumatların şəxsiyyət vəsiqəsi: Key-Value cütlükləri"

Bu gün Python-un ən güclü və çevik məlumat strukturlarından birini öyrənirik. **Dictionary** — sıralanmamış (Python 3.7+ versiyalarında sıralı), dəyişdirilə bilən və `key: value` (açar: dəyər) formatında işləyən bir kolleksiyadır.

---

## 🏗️ Lüğət Nədir?
Lüğəti fiziki bir lüğət kimi düşün: bir söz (key) və onun mənası (value).
*   **Key (Açar):** Unikal olmalıdır və dəyişməz (string, int, tuple) tipdə olmalıdır.
*   **Value (Dəyər):** İstənilən tipdə (list, set, hətta başqa bir lüğət) ola bilər.



---

## 🛠️ Əsas Əməliyyatlar (Dərsliyin Analizi)

### 1. Yaradılma və Ölçü
Lüğətlər fiqurlu mötərizə `{}` və ya `dict()` funksiyası ilə yaradılır.

```python
# Boş bir it lüğəti
dog = {} 

# Məlumatla dolu bir tələbə lüğəti
student = {
    'first_name': 'Elcan',
    'last_name': 'Kerimli',
    'skills': ['Python', 'Linux', 'Cybersecurity'],
    'address': {
        'city': 'Baku',
        'university': 'MAA'
    }
}
print(len(student)) # Cəmi 4 əsas key var
```

### 2. Elementlərə Giriş: Təhlükəsiz Yol
Elementə açar adı ilə müraciət edə bilərsən. Amma açar yoxdursa, proqram xəta (KeyError) verəcək. Bunun qarşısını almaq üçün `.get()` metodundan istifadə etmək daha peşəkarcadır.

```python
print(student['first_name']) # 'Elcan'
print(student.get('age'))    # None (Xəta vermir, proqram dayanmır)
```

### 3. Əlavə Etmə və Dəyişmə
Lüğətlər **mutable**-dır, yəni onları istənilən vaxt yeniləyə bilərsən.

```python
student['age'] = 19 # Yeni key əlavə edildi
student['first_name'] = 'Elcan (Digital Lawyer)' # Mövcud dəyər yeniləndi
```

### 4. Silmə Metodları
*   `pop(key)`: Müəyyən açarı və onun dəyərini silir.
*   `popitem()`: Sonuncu əlavə edilən elementi silir.
*   `del`: Spesifik bir açarı və ya bütün lüğəti yaddaşdan silir.
*   `clear()`: Lüğətin içini tamamilə boşaldır.

---

## 🔍 Lüğət Metodlarının Kəşfi

| Metod | Nəticə |
| :--- | :--- |
| `.keys()` | Bütün açarların siyahısını qaytarır. |
| `.values()` | Bütün dəyərlərin siyahısını qaytarır. |
| `.items()` | `(key, value)` formatında tuple siyahısı qaytarır. |
| `.copy()` | Orijinal lüğəti qorumaq üçün onun nüsxəsini yaradır. |

---

## 💻 Gün 08: Tapşırıqlar (Laboratoriya)

1.  **Dog Dictionary:** `dog` adlı boş lüğət yarat və ona `name`, `color`, `breed`, `legs`, `age` açarlarını əlavə et.
2.  **Student Dictionary:** Öz məlumatlarınla (ad, cins, yaş, bacarıqlar, ölkə və s.) bir `student` lüğəti yarat.
3.  **Data Analizi:**
    *   Tələbə lüğətinin uzunluğunu tap.
    *   `skills` dəyərini götür və onun tipinin `list` olduğunu yoxla.
4.  **Transformasiya:**
    *   Lüğətin açarlarını və dəyərlərini ayrı-ayrı siyahı kimi götür.
    *   Lüğəti `items()` ilə tuple siyahısına çevir.
    *   Bir elementi sil və axırda lüğətlərdən birini tamamilə `del` ilə yox et.

---

### 🛡️ Kiber-Mütəxəssis Notu:
"Təsəvvür et ki, bir serverdə minlərlə istifadəçi var. `List` istifadə etsən, bir istifadəçini tapmaq üçün bütün siyahını gəzməlisən (O(n)). Amma `Dictionary` (Hash Table mexanizmi ilə işləyir) istifadə etsən, istifadəçi adını (key) yazan kimi onun bütün məlumatlarını saniyənin mində biri qədər sürətlə tapacaqsan. Bu, performansın açarıdır!"

---
**Təbriklər! 8-ci günü də uğurla tamamladın.** 🎉 

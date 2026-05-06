
---

# 📅 Gün 05: Listlər (Siyahılar)

Python-da siyahılar birdən çox məlumatı tək bir dəyişəndə saxlamaq üçün istifadə olunur. Listlər **sıralanmış (ordered)** və **dəyişdirilə bilən (mutable)** kolleksiyalardır.

---

## 🏗️ 1. List Yaradılması
Siyahıları iki üsulla yarada bilərik:
1.  **Kvadrat mötərizə ilə:** `my_list = []`
2.  **`list()` funksiyası ilə:** `my_list = list()`

Siyahıların daxilində müxtəlif tip məlumatlar (string, int, bool, hətta başqa bir siyahı) ola bilər.



---

## 🔍 2. Elementlərə Giriş (Indexing & Slicing)

Elementləri onların mövqeyinə görə çağırırıq:
*   **Müsbət İndeksləmə:** 0-dan başlayaraq soldan sağa.
*   **Mənfi İndeksləmə:** -1-dən başlayaraq sağdan sola (sondakı elementi tapmaq üçün rahatdır).
*   **Slicing (Kəsmə):** `list[start:stop:step]` formatında siyahının müəyyən bir hissəsini götürmək olar.

```python
techs = ['Python', 'Linux', 'Kali', 'Go']
print(techs[0])    # 'Python'
print(techs[-1])   # 'Go'
print(techs[1:3])  # ['Linux', 'Kali']
```

---

## 🛠️ 3. Siyahı Üzərində Əməliyyatlar (Metodlar)

Siyahıları idarə etmək üçün bu metodlar mütləqdir:

| Metod | Funksiyası |
| :--- | :--- |
| `append(item)` | Siyahının **sonuna** yeni element əlavə edir. |
| `insert(index, item)` | Müəyyən edilmiş **mövqeyə** element yerləşdirir. |
| `remove(item)` | Göstərilən elementi siyahıdan silir. |
| `pop(index)` | Müəyyən indeksdəki elementi silir və onu bizə qaytarır. |
| `extend(list2)` | Bir siyahını digərinin sonuna birləşdirir. |
| `sort()` | Siyahını əlifba və ya rəqəm sırası ilə düzür. |
| `reverse()` | Siyahının ardıcıllığını tərsinə çevirir. |

---

## 📦 4. Unpacking (Siyahını Açma)
Siyahıdakı elementləri birbaşa dəyişənlərə mənimsədə bilərik:

```python
countries = ['Azerbaijan', 'Turkey', 'Germany']
az, tr, de = countries
# Və ya ulduz (*) operatoru ilə:
first, *others = ['A', 'B', 'C', 'D']
# first = 'A', others = ['B', 'C', 'D']
```

---

## 💻 Gün 05 - Praktik Tapşırıqlar (Laboratoriya)

### Səviyyə 1
1.  Boş bir siyahı yarat.
2.  İçində 5-dən çox IT şirkəti olan `it_companies` siyahısı yarat.
3.  Siyahının uzunluğunu tap.
4.  Siyahıya yeni bir şirkət `append` et.
5.  Siyahının tən ortasındakı şirkəti `insert` metodu ilə dəyiş.
6.  Siyahını əlifba sırası ilə düz.

### Səviyyə 2
1.  Aşağıdakı yaş siyahısını analiz et: `ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]`
    *   Siyahını sort et və minimum/maksimum yaşı tap.
    *   Orta yaşı (average) hesabla (cəmi / saya böl).
    *   Yaş diapazonunu (max - min) tap.

---

### 🛡️ Kiber-Təhlükəsizlik Notu:
" **List Comprehension** mövzusuna xüsusi diqqət yetir (Məsələn: `[x for x in range(10)]`). Bu, gələcəkdə böyük port skan nəticələrini və ya `log` fayllarını bir sətirdə filtrdən keçirmək üçün sənə inanılmaz sürət qazandıracaq. Unutma, siyahılar sənə həm də hədəf IP-lər siyahısını (target list) idarə etmək üçün lazımdır!"

---
🎉 **Təbriklər! 5-ci günü də uğurla tamamladın!** 🎉

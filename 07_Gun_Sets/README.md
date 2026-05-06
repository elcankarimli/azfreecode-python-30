---

# 📘 AzFreeCode: Gün 07 — Sets (Çoxluqlar)
### "Təkrarçılığa son: Unikal dataların qala qapısı"

Xoş gəldin! Bu gün Python-un riyazi tərəfi ilə tanış olacağıq. **Set** (Çoxluq) — sırasız, indekslənməyən və ən əsası **yalnız unikal elementlərdən** ibarət olan kolleksiyadır.

---

## 🛠️ Set Nədir? (Əsas Xüsusiyyətlər)

1.  **Unikallıq:** Eyni elementi iki dəfə əlavə edə bilməzsən. Təkrarlar avtomatik silinir.
2.  **Sırasızlıq:** Elementlərin xüsusi bir ardıcıllığı yoxdur. Hər çap edəndə yerləri dəyişə bilər.
3.  **İndekssizlik:** `st[0]` deyib element çağıra bilməzsən.
4.  **Dəyişkənlik (Mutable):** Set-in özünə yeni elementlər əlavə edib silə bilərsən, amma daxilindəki elementləri birbaşa redaktə edə bilməzsən.

---

## 🏗️ Set Əməliyyatları (Manual)

### 1. Yaradılma
Boş bir set yaratmaq üçün mütləq `set()` funksiyasından istifadə etməlisən. Boş fiqurlu mötərizə `{}` lüğət (dictionary) yaradır.

```python
# Boş set
st = set()

# İlkin dəyərlərlə
it_companies = {'Google', 'Facebook', 'Apple'}
```

### 2. Element Əlavə Etmə və Silmə
*   **`add(item)`**: Tək bir element əlavə edir.
*   **`update(list)`**: Çoxlu sayda elementi (məsələn, bir listi) set-ə əlavə edir.
*   **`remove(item)`**: Elementi silir. Tapmasa **Error** verir.
*   **`discard(item)`**: Elementi silir. Tapmasa Error **vermir** (daha təhlükəsizdir).
*   **`pop()`**: Təsadüfi bir elementi silir və onu sənə qaytarır.

---

## 🧬 Riyazi Set Əməliyyatları (Kiber-Analiz üçün)

İki set arasındakı əlaqəni tapmaq üçün bu metodlar əvəzsizdir:

| Əməliyyat | Metod / Operator | İzahı |
| :--- | :--- | :--- |
| **Birləşmə** | `union()` və ya `\|` | Hər iki set-dəki bütün unikal elementlər. |
| **Kəsişmə** | `intersection()` və ya `&` | Yalnız hər iki set-də olan ortaq elementlər. |
| **Fərq** | `difference()` və ya `-` | Birinci set-də olub, ikincidə olmayanlar. |
| **Simmetrik Fərq** | `symmetric_difference()` və ya `^` | Ortaq olanlar çıxılmaqla qalan bütün elementlər. |

---

## ❄️ Frozen Sets (Donmuş Çoxluqlar)
Əgər bir set-in tamamilə dəyişməz (immutable) olmasını istəyirsənsə, `frozenset()` istifadə edirsən. Bu, kiber-təhlükəsizlikdə sabit qara siyahılar (blacklists) yaratmaq üçün idealdır.

---

## 💻 Gün 07: Tapşırıqlar (Level 1, 2 və 3)

### Səviyyə 1
1.  `it_companies` setinin uzunluğunu tap.
2.  Siyahıya 'Twitter' əlavə et.
3.  Eyni anda 3 yeni şirkət əlavə et (`update` ilə).

### Səviyyə 2 (Məntiqi Əməliyyatlar)
```python
A = {19, 22, 24, 20, 25, 26}
B = {19, 22, 20, 25, 26, 24, 28, 27}

# 1. A və B-ni birləşdir
print(A.union(B))

# 2. A kəsişmə B-ni tap
print(A.intersection(B))

# 3. A, B-nin alt çoxluğudur (subset)?
print(A.issubset(B))
```

### Səviyyə 3 
1.  Aşağıdakı yaş siyahısını set-ə çevir: `age = [22, 19, 24, 25, 26, 24, 25, 24]`. Siyahınınmı, yoxsa set-inmi ölçüsü daha böyükdür? (İpucu: Set təkrarları silir).
2.  **Cümlə Analizi:** "I am a teacher and I love to inspire and teach people."
    *   Bu cümlədə neçə **unikal** söz var?
    *   `split()` metodu ilə sözlərə ayır, sonra `set()`-ə çevir və sayını tap.

---

### 🛡️ Qeyd
"Təsəvvür et ki, sənə minlərlə şəxsin giriş loqları (logs) verilib. Sənə sadəcə neçə nəfərin (unikal şəxs) sistemə girdiyini tapmaq lazımdır. `List` istifadə etsən, hər kəsi tək-tək saymalı olacaqsan. Amma həmin siyahını birbaşa `Set`-ə çevirsən, Python bütün təkrarları (eyni şəxsin 100 dəfə girməsini) bir saniyədə siləcək və sənə təmiz siyahını verəcək!"

---
**7-ci günü də uğurla bitirdik!** Bu sürətlə getsən, 30 günün sonunda əsl Python ustası olacaqsan. 8-ci gün **Dictionaries (Lüğətlər)** bizi gözləyir. Hazırsan? 🚀

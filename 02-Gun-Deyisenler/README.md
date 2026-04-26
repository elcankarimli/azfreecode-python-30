

# 📅 Gün 2: Dəyişənlər və Daxili Funksiyalar

Python-un gücü onun sadəliyində və çevikliyindədir. Bu gün biz məlumatları necə yadda saxlayacağımızı (Dəyişənlər) və Python-un bizə təqdim etdiyi hazır alətləri (Daxili Funksiyalar) öyrənəcəyik.

---

## 🏗️ 1. Dəyişənlər (Variables) Nədir?

Dəyişənlər məlumatları kompüterin yaddaşında saxlamaq üçün istifadə olunan etiketlərdir. Onları daxilində dəyər saxlayan "etiketli qutular" kimi təsəvvür edə bilərsiniz.



### 🐍 Python-da Dəyişən Adlandırma Qaydaları
Peşəkar kod yazmaq üçün bu qaydalara əməl etmək mütləqdir:
* **Snake Case:** Python tərtibatçıları çoxsözlü dəyişənlər üçün `alt_xətt` istifadə edirlər (məs: `menim_adim`, `istifadeci_yasi`).
* **Rəqəmlə başlaya bilməz:** `1num` olmaz, laktin `num1` olar.
* **Xüsusi simvollar:** `@`, `$`, `-` kimi simvollar istifadə edilə bilməz.
* **Case-Sensitive:** `age`, `Age` və `AGE` üç fərqli dəyişəndir.
* **Rezerv olunmuş sözlər:** `if`, `class`, `def` kimi Python-un özünə aid sözləri dəyişən adı kimi istifadə etmək olmaz.

### 💡 Birdən çox dəyişəni bir sətirdə elan etmək:
```python
ad, soyad, yas = 'Elcan', 'Karimli', 17
```

---

## 🛠️ 2. Daxili Funksiyalar (Built-in Functions)

Python bizə heç bir kitabxana yükləmədən istifadə edə biləcəyimiz çoxlu hazır funksiyalar təqdim edir.

| Funksiya | Təsviri |
| :--- | :--- |
| `print()` | Məlumatı terminala çıxarır. Vergüllə bir neçə arqument ala bilər. |
| `len()` | Sətir və ya siyahıdakı elementlərin sayını (uzunluğunu) qaytarır. |
| `type()` | Verilən dəyişənin hansı data tipinə aid olduğunu göstərir. |
| `input()` | İstifadəçidən birbaşa məlumat qəbul edir (həmişə **string** qaytarır). |
| `isinstance()` | Obyektin müəyyən bir tipə aid olub-olmadığını yoxlayır (True/False). |

---

## 📊 3. Məlumat Tipləri və Dinamik Tipləşmə

Python **dinamik tipləşən (dynamically-typed)** dildir. Bu o deməkdir ki, siz dəyişənin tipini əvvəlcədən bildirmirsiniz (`int age = 25` yerinə sadəcə `age = 25`). Python dəyərə baxaraq tipi özü təyin edir.

### Əsas Məlumat Tipləri:
* **Integer:** Tam ədədlər (10, -5).
* **Float:** Onluq kəsrlər (3.14, 9.81).
* **String:** Dırnaq daxilində yazılan mətnlər ('Salam').
* **Boolean:** Məntiqi dəyərlər (True, False).
* **Complex:** Kompleks ədədlər (1 + 1j).
* **None:** Dəyərin yoxluğunu təmsil edən xüsusi tip.

### 🔄 Tip Çevirmə (Casting)
Bəzən bir tipi digərinə çevirmək lazım gəlir:
```python
num_str = '10'
num_int = int(num_str)  # String-dən Integer-ə
num_float = float(10)   # 10.0
```

---

## 🏢 4. Sənaye Tətbiqi və DevOps

* **DevOps:** Python dəyişənləri və skriptləri infrastrukturun (məs: serverlərin) avtomatlaşdırılmasında, CI/CD boru kəmərlərinin idarə edilməsində geniş istifadə olunur.
* **Kibertəhlükəsizlik:** Sənayedə `print()` funksiyası loqların analizi üçün, `input()` isə interaktiv skan alətləri yaratmaq üçün istifadə edilir.

---

## 💻 2-ci Günün Tapşırıqları

### Səviyyə 1
1. `day_2` qovluğunda `variables.py` faylı yarat.
2. Ad, soyad, ölkə, şəhər, yaş və `is_married` dəyişənlərini elan et.
3. Bir sətirdə birdən çox dəyişən elan etməyi sına.

### Səviyyə 2
1. `type()` funksiyası ilə bütün dəyişənlərinin tipini yoxla.
2. `len()` funksiyası ilə adının uzunluğunu tap və soyadının uzunluğu ilə müqayisə et.
3. Riyazi əməliyyatlar: `num_one = 5`, `num_two = 4` götürərək cəmini, fərqini, hasilini, bölünməsini və qüvvətini tap.
4. **Dairənin Sahəsi:** İstifadəçidən radiusu alaraq dairənin sahəsini hesablayan proqram yaz ($Area = \pi \times r^2$).
5. `help('keywords')` komandasını işlədərək Python-un qadağan olunmuş açar sözlərinə bax.

---
**Təbriklər! 2-ci günü də uğurla tamamladın. Artıq Python-un yaddaşını idarə edə bilirsən! 🚀**

# AZFREECODE:Öyrən,Tətbiq et,Paylaş!
#Azfreecode


---



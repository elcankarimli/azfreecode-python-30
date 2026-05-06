---

# 🛡️ AzFreeCode: Gün 06 — Tuples (Kortecələr)
### "Sözü bir, özü bütöv məlumat strukturları"

Xoş gəldiniz! Bu gün Python-un **"əsas mövuzlardan"** olan Tuples mövzusuna daxil oluruq. Əgər Listlər hər gün dəyişən bir "vatsap statusu"dursa, Tuples — üzərində dövlət möhürü olan bir "diplom"dur. Bir dəfə yazıldısa, bitdi!

---

## 🧐 Tuple Nədir? (Hüquqi və Texniki Baxış)

Python-da **Tuple** — sıralanmış, lakin **immutable** (dəyişdirilə bilməz) məlumat kolleksiyasıdır. Bir kiber-mütəxəssis üçün bu, "read-only" (yalnız oxuna bilən) fayl sistemi kimidir.



### ⚖️ Niyə List deyil, Tuple?
1.  **Prinsipləri:** Tuple-da olan elementləri silə, dəyişə və ya yenisini əlavə edə bilməzsən. Bu, datanın bütövlüyünü (integrity) qoruyur.
2.  **Sürət:** Proqram işləyərkən Python Tuple-ları List-lərdən daha sürətli emal edir.
3.  **Yaddaş Qənaəti:** Daha az RAM sərf edir, bu da laptopunda minlərlə data ilə işləyəndə fərq yaradır.

---

## 🛠️ Tuple Əməliyyatları (Cheat Sheet)

### 1. Yaradılma: "Möhürün Vurulması"
```python
# Boş bir qanun kitabı
empty_tpl = () 

# Kiber-təhlükəsizlik alətləri (Dəyişməz siyahı)
tools = ('Nmap', 'Metasploit', 'Wireshark') 

# DİQQƏT: Tək elementli Tuple-da vergül mütləqdir!
single_law = ("Qanun 1",) 
```

### 2. Elementlərə Giriş: "Maddə Analizi"
Siyahılarda olduğu kimi, indeksləmə 0-dan başlayır.
*   `tools[0]` -> `'Nmap'`
*   `tools[-1]` -> `'Wireshark'` (Sonuncu maddə)



### 3. Unpacking: "Bağlamanı Sökmək"
Bu hissə ən əyləncəli yerdir. Bir Tuple-ı saniyələr içində ayrı-ayrı dəyişənlərə parçalaya bilərsən:
```python
db_config = ("xxx.xxx.x.x", "admin", "root123")
ip, user, password = db_config

print(ip) # "xxx.xxx.x.x"
```

---

## 🔓 "Sistemi Aldatmaq": Tuple Necə Dəyişdirilir?

Normalda Tuple dəyişmir. Amma bir hacker kimi "arxa qapıdan" daxil ola bilərik:
1.  Tuple-ı **List**-ə çevir: `list_version = list(my_tuple)`
2.  İstədiyin dəyişikliyi et (maddəni redaktə et).
3.  Yenidən **Tuple**-a çevir: `my_tuple = tuple(list_version)`

---

## 💻 Gün 06: Laboratoriya İşləri

### 🧪 Səviyyə 1: Ailə Arxivləri
1.  Boş bir tuple yarat.
2.  Xəyali (və ya real) qardaş və bacılarının adlarından ibarət iki ayrı tuple yarat.
3.  Onları `siblings` adlı bir tuple-da birləşdir (`+` operatoru ilə).
4.  `len()` funksiyası ilə neçə nəfər olduğunuzu öyrən.
5.  Ata və ananın adını bu tuple-a "arxa qapı" (list-ə çevirmə) yolu ilə əlavə et.

### 🧪 Səviyyə 2: Data Analitikası
1.  Aşağıdakı tuple-ı yarat:
    `nordic_countries = ('Denmark', 'Finland', 'Iceland', 'Norway', 'Sweden')`
2.  Yoxla: 'Estonia' bu siyahıdadır? (Cavab `False` çıxmalıdır).
3.  Yoxla: 'Iceland' bu siyahıdadır? (Cavab `True` çıxmalıdır).

---

## 📝 Yekun Qeyd
> "Məlumatın dəyişməsini istəmirsənsə, onu Tuple-a həbs et!"

Bu gün siz Python-da datanın toxunulmazlığını öyrəndiniz. Sabah isə **Sets (Çoxluqlar)** dünyasına, yəni təkrarlanan məlumatların qəbul edilmədiyi "filtr" sisteminə keçəcəyik!

---
**Keçək 7-ci günə! 🚀**



 
### AzFreeCode: Gün 10 — Loops (Dövrlər)

Proqramlaşdırmada təkrarlanan tapşırıqları yerinə yetirmək üçün dövrlərdən istifadə olunur. Python bizə iki əsas dövr növü təklif edir: `while` və `for`.



## 🔄 1. While Dövrü
`while` dövrü müəyyən bir şərt **True** olduğu müddətcə işləməyə davam edir. Şərt **False** olan kimi dövr dayanır.
```python
count = 0
while count < 5:
    print(f"Sayı: {count}")
    count = count + 1  # Bu sətir olmasa dövr sonsuz olar!
```

---

## 🏎️ 2. For Dövrü
`for` dövrü daha çox siyahılar (list), lüğətlər (dict) və ya simvolların (string) üzərindən keçmək üçün istifadə olunur.

```python
tech_tools = ['Nmap', 'Burp Suite', 'Metasploit']
for tool in tech_tools:
    print(f"Alət: {tool}")
```

### 🎯 Range() Funksiyası
Müəyyən sayda təkrar etmək üçün `range()` funksiyasından istifadə edirik:
```python
for i in range(5):  # 0-dan 4-ə qədər (5 daxil deyil)
    print(i)
```

---

## 🎮 Dövrü İdarə Edən Komandalar: Break və Continue

* **Break:** Şərt ödənmədən belə dövrü dərhal dayandırır və çıxır.
* **Continue:** Cari addımı ötürür və dövrün növbəti addımına keçir.

```python
for i in range(10):
    if i == 3:
        continue  # 3-ü ötürür
    if i == 7:
        break     # 7-yə çatanda tamamilə dayanır
    print(i)
```

---

## 🧱 İç-içə (Nested) Dövrlər
Bir dövrün daxilində başqa bir dövr yaza bilərik. Məsələn, bir cədvəl qurmaq üçün:

```python
for i in range(1, 4):
    for j in range(1, 4):
        print(f"({i}, {j})", end=" ")
    print() # Növbəti sətir üçün
```

---

## 💻 Gün 10: Tapşırıqlar (Laboratoriya)

### Səviyyə 1
1.  0-dan 10-a qədər həm `for`, həm də `while` ilə çap et.
2.  Ekranda aşağıdakı üçbucağı yaradan bir dövr yaz:
    ```
    #
    ##
    ###
    ####
    ```
3.  ['Python', 'Numpy', 'Pandas'] siyahısını dövrə salaraq elementləri çap et.

### Səviyyə 2
1.  0-dan 100-ə qədər olan bütün ədədlərin cəmini tapan kod yaz. (Nəticə: 5050)
2.  0-dan 100-ə qədər olan yalnız cüt ədədlərin cəmini tap.

### Səviyyə 3 (Data Analizi)
1.  Bir meyvə siyahısı yarat və dövr vasitəsilə həmin siyahını tərsinə çevir.
2.  (Könüllü) Əgər bir ölkələr siyahın varsa, adı "land" ilə bitən ölkələri (məsələn: Finland, Iceland) dövr ilə seçib yeni bir siyahıya yığ.

---

### 🛡️ Cyber-Police & Forensics Note:
"Dostlar, təsəvvür edin ki, bir kiber-hücum olub və əlinizdə 1 milyon sətirlik 'log' faylı var. Bu faylda hansı saatda sistemə kənar müdaxilə olduğunu tapmaq üçün `for` dövrü və daxilində bir `if` şərti kifayətdir. İnsan gözünün saatlarla edə bilməyəcəyi analizi, düzgün qurulmuş bir dövr millisanisəyə həll edir. Avtomatlaşdırmanın gücü budur!"

---
**TƏBRİKLƏR 10-CU GÜNÜ TAMAMLADIN!**

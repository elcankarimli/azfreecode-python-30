---

# 📘 AzFreeCode: Gün 09 — Conditionals (Şərt Operatorları)
### "Kodunuzun beyni: Qərar vermə məntiqi"

Normalda Python kodları yuxarıdan aşağıya ardıcıl icra olunur. Lakin həyatda olduğu kimi, proqramlaşdırmada da bəzən seçim etmək lazım gəlir. Şərt operatorları bizə bu axını idarə etmək imkanı verir.



---

## 🚦 1. If (Əgər) Şərti
Ən sadə formadır. Əgər verilən şərt **True** (doğru) olarsa, həmin blokdakı kod icra olunur.

```python
# Sintaksis
if şərt:
    icra olunacaq kod
```

> **Vacib Qeyd:** Python-da ":" işarəsindən sonra mütləq **indentation** (boşluq/girinti) qoyulmalıdır. Bu, kodun o şərtə aid olduğunu göstərir.

---

## 🛤️ 2. If Else (Əks halda)
Əgər şərt doğru deyilsə, alternativ bir yol göstərmək üçün istifadə olunur.

```python
age = 15
if age >= 18:
    print("Siz səs verə bilərsiniz.")
else:
    print("Səs vermək üçün yaşınız çatmır.")
```

---

## 🪜 3. If Elif Else (Çoxşaxəli qərarlar)
Gündəlik həyatda sadəcə iki deyil, çoxlu seçimimiz olur. Məsələn, tələbənin balına görə qiymət verərkən `elif` (else if) istifadə edirik.

```python
score = 85
if score >= 90:
    print("Qiymət: A")
elif score >= 80:
    print("Qiymət: B")
elif score >= 70:
    print("Qiymət: C")
else:
    print("Qiymət: F")
```

---

## ⚡ Qısa Yol (Short Hand / Ternary Operator)
Əgər şərtiniz çox sadədirsə, onu bir sətirdə yaza bilərsiniz.

```python
a = 3
print('Müsbət') if a > 0 else print('Mənfi')
```

---

## 🖇️ Məntiqi Operatorlarla İstifadə (And, Or)
Bəzən bir neçə şərtin eyni anda ödənməsini (`and`) və ya ən azı birinin ödənməsini (`or`) istəyirik.

*   **And:** Hər iki şərt doğru olmalıdır.
*   **Or:** Şərtlərdən biri doğru olsa kifayətdir.

```python
user = 'admin'
access_level = 3
if user == 'admin' or access_level >= 4:
    print("Girişə icazə verildi!")
else:
    print("Giriş qadağandır!")
```

---

## 💻 Gün 09: Tapşırıqlar (Beyin Məşqi)

### Səviyyə 1
1.  İstifadəçidən yaşını soruş (`input`). Əgər 18-dən böyükdürsə "Sürücülük vəsiqəsi ala bilərsən", deyilsə neçə il gözləməli olduğunu çap et.
2.  `my_age` və `your_age` dəyişənlərini müqayisə et. Kimin böyük olduğunu və aradakı il fərqini tap.

### Səviyyə 2
1.  **Qiymətləndirmə sistemi:** 90-100 (A), 80-89 (B), 70-79 (C), 60-69 (D), 0-59 (F) formatında kod yaz.
2.  **Fəsil təyini:** İstifadəçi ay adını yazsın (məsələn, "Sentyabr"), proqram hansı fəsil (Payız, Qış, Yaz, Yay) olduğunu desin.

### Səviyyə 3 (Mürəkkəb Analiz)
Aşağıdakı `person` lüğəti üzərində işlə:
*   Əgər şəxsin bacarıqları arasında 'Python' varsa, bunu qeyd et.
*   Əgər yalnız 'JavaScript' və 'React' bilirsə "Front-end developer", 'Node' və 'Python' bilirsə "Back-end developer" olduğunu çap et.

---

### 🛡️ Digital Lawyer & Security Insight:
"Dostlar, kiber-təhlükəsizlikdə **'Firewall'** (təhlükəsizlik divarı) dediyimiz şey əslində nəhəng bir `if-else` blokudur. `if incoming_packet == 'malicious': block()` — proqram təminatı hər saniyə milyonlarla belə qərar verir. Bu gün öyrəndiyiniz bu sadə məntiq, dünyanın ən böyük sistemlərinin təhlükəsizliyini qoruyan təməl daşıdır!"

---
**Təbriklər !** 9-cu günü də uğurla tamamladın. 🎉 10-cu gündə **Loops (Dövrlər)** mövzusuna keçib kodlarımızı təkrar-təkrar işlətməyi öyrənəcəyik. 🚀

---

### 🚀 Python-da "İş Görən" Operatorlar: Nədir, Nə İşə Yarayır?

Dostlar, təsəvvür edin ki, Python bir fabrikdir. Dəyişənlər (variables) bu fabrikdəki qutulardır, içində məlumatlar var. **Operatorlar** isə o qutuları götürüb bir-birinə vuran, içindəkiləri ölçən-biçən işçilər və maşınlardır.

#### 1. "Hesabdar" Operatorlar (Arifmetik)
Burada riyaziyyatdan bildiyimiz toplama-çıxma var, amma Python-un bəzi "hiylələri" mövcuddur:
*   **`7 / 2` vs `7 // 2`**: Birincisi sənə tam dəqiqliyi verir (3.5), ikincisi isə "mənə kəsr lazım deyil, neçə dənə tam yerləşir?" deyir (3).
*   **Qalıq tapmaq (`%`)**: Bu proqramlaşdırmanın gizli qəhrəmanıdır. Bir ədəd digərinə tam bölünürmü? Cütdürmü? Təkdirmi? Hamısını bu balaca faiz işarəsi ilə tapırıq.



#### 2. "Tərəzi" Operatorlar (Müqayisə)
Bax, bu hissə proqramın "beyni"dir. Proqram burada qərar verir.
*   **`==`**: "Dostum, bu iki şey həqiqətən eynidirmi?" deyə soruşur. (Məsələn: Daxil edilən parol sistemdəki ilə eynidir?)
*   **`!=`**: "Bunlar fərqli olsun!" deyir.
*   **`>` , `<`**: "Kimin gücü (dəyəri) daha çoxdur?" sualını verir.

> **Unutma:** Bu operatorların cavabı həmişə ya **True (Hə)**, ya da **False (Yox)** olur. Orta variant yoxdur!

#### 3. "Vəkil" Operatorlar (Məntiqi)
Mürəkkəb vəziyyətlərdə bunlar köməyə çatır:
*   **`and`**: Çox tələbkardır. "Həm boyun 170-dən yuxarı olsun, həm də çəkin 70-dən aşağı olsun" deyir. Biri olmasa, keçid vermir.
*   **`or`**: Daha səmimidir. "Ya tələbə biletin olsun, ya da şəxsiyyət vəsiqən, hər ikisi ilə girə bilərsən" deyir.
*   **`not`**: Tam bir inadkardır. Nə desən, tərsinə çevirir. `not True` (Doğru deyil) desən, sənə `False` qaytarar.

---

### 🔥 Tələbələr üçün nümunə:

Gəl bir "Hacker" ssenarisi quraq. Sistemin giriş şərti belədir:

```python
is_admin = True
is_verified = False

# Giriş üçün ya admin olmalısan, ya da hesabı təsdiqləməlisən.
# Amma gərək hər ikisi eyni anda False (Yalan) olmasın.
can_login = is_admin or is_verified

print("Giriş icazəsi:", can_login) # Cavab True olacaq, çünki bir dənə 'or' (və ya) bəs edir!
```

---

### 💻 Praktik Tapşırıq 


"Təsəvvür edin ki, bir proqram yazmalısınız. İstifadəçi yaşını girir. Əgər yaşı **18-dən böyükdürsə** VƏ **sürücülük vəsiqəsi varsa**, ekrana 'Maşın sürə bilərsən' yazsın."

Bunu kodla necə yazarıq?
`if age > 18 and has_license == True:`

---



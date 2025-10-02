# **Dasturlash Tillarining Asosiy Elementlari**

## **Kirish**

Hurmatli o'quvchilar! Bugun biz dasturlash tillarining asosiy qismlari bilan tanishamiz. Xuddi inson tillarida so'zlar, qoida va iboralar bo'lgani kabi, dasturlash tillarining ham o'ziga xos "so'z boyligi" va "grammatikasi" mavjud. Keling, ularni batafsil o'rganamiz.

---

## **1. O'zgaruvchilar (Variables)**

### **Nima bu?**
O'zgaruvchi - bu ma'lumotlarni saqlash uchun mo'ljallangan joy. Xotirada ma'lum bir joyni egallaydi va unga nom beriladi.

### **Qanday ishlaydi?**
```python
ism = "Ali"
yosh = 15
baholar = [5, 4, 5]
```

### **Hayotiy misol:**
Portfelingizni o'ylab ko'ring:
- **Portfel** - xotira
- **Qalamquti** - `qalamlar` o'zgaruvchisi
- **Daftar** - `dars_daftari` o'zgaruvchisi
- **Kalkulyator** - `hisoblagich` o'zgaruvchisi

Har bir narsa o'z joyida saqlanadi va kerak bo'lganda olinadi.

---

## **2. Ma'lumot Turlari (Data Types)**

### **Asosiy turlari:**

#### **a) Butun Sonlar (Integer)**
- **Ma'nosi:** Kasrsiz raqamlar
- **Misollar:** `15`, `-3`, `0`, `1000`
- **Hayotiy misol:** Sinfdagi o'quvchilar soni, sizning yoshingiz

#### **b) Haqiqiy Sonlar (Float)**
- **Ma'nosi:** Kasrli raqamlar
- **Misollar:** `3.14`, `-2.5`, `9.8`
- **Hayotiy misol:** Bo'yingiz (1.65 m), choyning harorati (85.5°C)

#### **c) Matn (String)**
- **Ma'nosi:** Belgilar ketma-ketligi
- **Misollar:** `"Salom"`, `'Dunyo'`, `"123"`
- **Diqqat:** Har doim qo'shtirnoq ichida yoziladi
- **Hayotiy misol:** Do'stingizga yuboradigan SMS, kitobdagi matn

#### **d) Mantiqiy Qiymatlar (Boolean)**
- **Ma'nosi:** Faqat ikkita qiymat: `True` (rost) yoki `False` (yolg'on)
- **Misollar:** `True`, `False`
- **Hayotiy misol:** 
  - Chiroq yoqilganmi? (`True`/`False`)
  - Dars boshlandimi? (`True`/`False`)

#### **e) Ro'yxatlar (List)**
- **Ma'nosi:** Bir nechta elementlarning tartiblangan to'plami
- **Misollar:** `["olma", "banan", "nok"]`, `[1, 2, 3, 4, 5]`
- **Hayotiy misol:** Sinfdagi barcha o'quvchilar ismlari ro'yxati

---

## **3. Operatorlar (Operators)**

### **a) Arifmetik Operatorlar**
| Operator | Nomi | Misol | Natija |
|----------|-------|--------|---------|
| `+` | Qo'shish | `5 + 3` | `8` |
| `-` | Ayirish | `10 - 4` | `6` |
| `*` | Ko'paytirish | `6 * 2` | `12` |
| `/` | Bo'lish | `15 / 3` | `5.0` |
| `%` | Qoldiq | `17 % 5` | `2` |

### **b) Taqqoslash Operatorlari**
| Operator | Ma'nosi | Misol | Natija |
|----------|----------|--------|---------|
| `==` | Tengmi? | `5 == 5` | `True` |
| `!=` | Teng emasmi? | `5 != 3` | `True` |
| `>` | Kattami? | `10 > 5` | `True` |
| `<` | Kichikmi? | `3 < 7` | `True` |
| `>=` | Katta yoki tengmi? | `8 >= 8` | `True` |
| `<=` | Kichik yoki tengmi? | `6 <= 10` | `True` |

### **c) Mantiqiy Operatorlar**
| Operator | Ma'nosi | Misol | Natija |
|----------|----------|--------|---------|
| `and` | VA | `(5 > 3) and (2 < 4)` | `True` |
| `or` | YOKI | `(5 > 3) or (2 > 4)` | `True` |
| `not` | Yo'q/Inkor | `not (5 > 3)` | `False` |

**Hayotiy misol:**
```python
# Do'kondan non sotib olish shartlari
pul_bormi = True
doqon_ochiqmi = True

if pul_bormi and doqon_ochiqmi:
    print("Non sotib olish mumkin")
else:
    print("Non sotib olib bo'lmaydi")
```

---

## **4. Shart Operatorlari**

### **a) if-else operatori**
```python
# Oddiy misol
yomgir_yogyaptimi = True

if yomgir_yogyaptimi:
    print("Soyabon oling!")
else:
    print("Quyoshdan ko'zoynak oling!")
```

### **b) Ko'p shartli tekshirish**
```python
baho = 4

if baho == 5:
    print("A'lo!")
elif baho == 4:
    print("Yaxshi!")
elif baho == 3:
    print("Qoniqarli!")
else:
    print("Qoniqarsiz!")
```

**Hayotiy misol - svetofor:**
```python
svetofor_rangi = "yashil"

if svetofor_rangi == "qizil":
    print("To'xtang!")
elif svetofor_rangi == "sariq":
    print("Tayyorlaning!")
else:  # yashil
    print("Yuring!")
```

---

## **5. Takrorlash Operatorlari (Sikllar)**

### **a) for tsikli**
- **Ma'nosi:** Ma'lum bir necha marta takrorlash

```python
# Misol 1: Ro'yxat elementlarini chiqarish
meyvalar = ["olma", "banan", "nok"]
for meyva in meyvalar:
    print(meyva)

# Misol 2: Belgili sonlar oralig'ida
for son in range(1, 6):
    print(son)
```

**Hayotiy misol:** Har bir o'quvchiga daftar tarqatish

### **b) while tsikli**
- **Ma'nosi:** Shart bajarilguncha takrorlash

```python
# Misol: 1 dan 5 gacha sonlarni chiqarish
son = 1
while son <= 5:
    print(son)
    son = son + 1
```

**Hayotiy misol:** Choy qaynaguncha kutish

---

## **6. Funktsiyalar (Functions)**

### **Nima bu?**
Funktsiya - ma'lum bir vazifani bajaradigan kod bo'lagi. Uni qayta-qayta chaqirish mumkin.

### **Funktsiya yaratish:**
```python
def salom_ber(ism):
    """Foydalanuvchiga salom beruvchi funktsiya"""
    print(f"Salom, {ism}!")

# Funktsiyani chaqirish
salom_ber("Ali")
salom_ber("Dilshoda")
```

### **Parametrli funktsiya:**
```python
def ikkiga_kopaytir(son):
    """Sonni ikkiga ko'paytiradi"""
    natija = son * 2
    return natija

# Funktsiyani chaqirish
javob = ikkiga_kopaytir(5)
print(javob)  # 10 chiqadi
```

**Hayotiy misol:** Oshxona retsepti
- **Funktsiya nomi:** `nonushta_tayyorla()`
- **Parametrlar:** `non_soni`, `choy_qaynatilsinmi`
- **Qaytaradigan natija:** Tayyor nonushta

---

## **7. Kutubxonalar va Modullar**

### **Nima bu?**
Kutubxona - oldindan tayyor funktsiyalar to'plami. Nima uchun velosipedni noldan yasaysizki, tayyori bor?

### **Misol kutubxonalar:**
```python
# Matematik kutubxona
import math
print(math.sqrt(16))  # 4.0 - kvadrat ildiz

# Tasodifiy sonlar kutubxonasi
import random
print(random.randint(1, 10))  # 1 va 10 orasida tasodifiy son

# Vaqt kutubxonasi
import datetime
bugun = datetime.datetime.now()
print(bugun)
```

**Hayotiy misol:** 
- **Kalkulyator** = `math` kutubxonasi
- **Tasodifiy raqamlar** = `random` kutubxonasi  
- **Soat/taqvim** = `datetime` kutubxonasi

---

## **Amaliy Misol: Barcha Elementlarni Qo'llash**

Keling, barcha o'rgangan elementlarimizdan foydalanib, oddiy dastur yozamiz:

```python
# O'quvchi baholarini hisoblovchi dastur

def baholarni_hisobla(ism, baholar):
    """O'quvchining o'rtacha bahosini hisoblaydi"""
    
    # O'rtacha bahoni hisoblash
    jami = 0
    for baho in baholar:
        jami = jami + baho
    
    o_rtacha = jami / len(baholar)
    
    # Baholash
    if o_rtacha >= 4.5:
        daraja = "A'lo"
    elif o_rtacha >= 3.5:
        daraja = "Yaxshi"
    elif o_rtacha >= 2.5:
        daraja = "Qoniqarli"
    else:
        daraja = "Qoniqarsiz"
    
    # Natijani qaytarish
    return f"{ism}ning o'rtacha bahosi: {o_rtacha:.1f} ({daraja})"

# Dastur asosiy qismi
o_quvchi_ismi = "Ali"
fan_baholari = [5, 4, 5, 3, 4]

natija = baholarni_hisobla(o_quvchi_ismi, fan_baholari)
print(natija)
```


---

## **Xulosa**

Bugun biz dasturlashning asosiy tarkibiy qismlarini o'rgandik:

1. **O'zgaruvchilar** - ma'lumotlarni saqlash
2. **Ma'lumot turlari** - qanday ma'lumotlar bilan ishlaymiz  
3. **Operatorlar** - ma'lumotlar ustida amallar bajarish
4. **Shart operatorlari** - qaror qabul qilish
5. **Takrorlash operatorlari** - bir xil ishlarni takrorlash
6. **Funktsiyalar** - kodni qayta ishlatish
7. **Kutubxonalar** - tayyor yechimlardan foydalanish

Bu elementlarning barchasi har qanday dasturlash tilida mavjud va ularni bilish sizga kelajakda murakkab dasturlar yozish imkoniyatini beradi.

**Eslab qoling:** Dasturlash - bu mantiqiy fikrlash va muammolarni ketma-ketlikda hal qilish san'ati!

---

*Keyingi darsimizda ushbu elementlarni amaliyotda qo'llashni o'rganamiz. Tayyor bo'ling!*
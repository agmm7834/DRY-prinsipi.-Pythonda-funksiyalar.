# Python Funksiyalar (DRY Prinsipi) - 20 ta Masala

## RETURNLI FUNKSIYALAR (1-10)

1. Berilgan sonning faktorialini hisoblaydigan funksiya yozing. Funksiya natijani qaytarsin.

2. Ikkita son orasidagi barcha juft sonlar yig'indisini hisoblaydigan funksiya yarating.

3. Ro'yxatdagi eng katta va eng kichik sonlarning o'rta arifmetigini qaytaruvchi funksiya yozing.

4. Matnni teskarisiga o'girib, palindrom ekanligini tekshiruvchi funksiya tuzing (True/False qaytaradi).

5. Berilgan sonning barcha raqamlari yig'indisini qaytaruvchi funksiya yarating. Masalan: 345 → 3+4+5 = 12

6. Ikki ro'yxatdagi umumiy elementlarni topib, yangi ro'yxat sifatida qaytaruvchi funksiya yozing.

7. Matndan barcha raqamlarni ajratib olib, ularning yig'indisini qaytaruvchi funksiya tuzing.

8. Berilgan ro'yxatdagi dublikatlarni o'chirib, noyob elementlardan iborat yangi ro'yxat qaytaruvchi funksiya yozing.

9. So'zning unlilar sonini hisoblaydigan funksiya yarating (a, e, i, o, u).

10. Ikkita lug'atni birlashtiruvchi funksiya yozing. Agar kalit takrorlansa, ikkinchi lug'at qiymatini olsin.

## RETURNSIZ FUNKSIYALAR (11-20)

11. Berilgan son jadvalini (ko'paytirish jadvali) 1 dan 10 gacha ekranga chiqaruvchi funksiya yozing.

12. Ro'yxatdagi barcha sonlarni kvadratga ko'taruvchi funksiya yarating (o'sha ro'yxatni o'zgartiradi).

13. Talaba ma'lumotlarini (ism, familiya, yosh, ball) qabul qilib, formatlangan holda ekranga chiqaruvchi funksiya tuzing.

14. Berilgan oraliqda (start, end) 5 ga bo'linadigan barcha sonlarni ekranga chiqaruvchi funksiya yozing.

15. Lug'atdagi barcha kalit va qiymatlarni chiroyli formatda (kalit: qiymat) ekranga chop etuvchi funksiya yarating.

16. Berilgan ro'yxatdagi barcha manfiy sonlarni 0 ga o'zgartiruvchi funksiya tuzing.

17. Foydalanuvchidan ism va yoshni so'rab, "Salom, [ism]! Siz [yosh] yoshdasiz." deb ekranga chiqaruvchi funksiya yozing.

18. Matnni berilgan belgi bilan kesib, har bir qismini yangi qatordan chiqaruvchi funksiya yarating.

19. Yulduzchalardan to'rtburchak chizuvchi funksiya tuzing (kenglik va balandlik parametr sifatida beriladi).

20. Ro'yxatdagi barcha string elementlarni katta harfga o'zgartiruvchi funksiya yozing (o'sha ro'yxatni o'zgartiradi).

---

**DRY Prinsipi eslatmasi:** Don't Repeat Yourself - kodingizni takrorlamaslik uchun funksiyalardan foydalaning. Bir xil amallarni turli joylarda yozish o'rniga, funksiya yaratib, uni chaqiring.

**Masalan:**
```
# Noto'g'ri (takrorlanish):
son1 = 5
if son1 % 2 == 0:
    print("Juft")
else:
    print("Toq")

son2 = 7
if son2 % 2 == 0:
    print("Juft")
else:
    print("Toq")

# To'g'ri (DRY):
def juft_toq(son):
    if son % 2 == 0:
        print("Juft")
    else:
        print("Toq")

juft_toq(5)
juft_toq(7)
```

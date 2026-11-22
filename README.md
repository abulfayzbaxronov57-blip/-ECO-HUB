# ECO-Hub

Maktab ekologiyasini boshqarish uchun Node.js + Express + SQLite asosidagi boshlang‘ich platforma.

## 1. Talablar

- Node.js 22.13 yoki undan yangi versiya (Node.js 26 ham mos).
- VS Code tavsiya etiladi.

SQLite Node.js ichidagi `node:sqlite` modulidan foydalanadi. Alohida database server o‘rnatish shart emas.

## 2. O‘rnatish

Terminalni loyiha papkasida oching:

```bash
npm install
npm run dev
```

Brauzerda quyidagi manzilni oching:

```text
http://localhost:3000
```

Serverni odatiy rejimda ishga tushirish:

```bash
npm start
```

## 3. Demo akkauntlar

Barcha xodim demo akkauntlari uchun parol: `EcoHub123!`

| Rol | Login |
|---|---|
| Eco Admin | admin@ecohub.local |
| Direktor | director@ecohub.local |
| Direktor o‘rinbosari | deputy@ecohub.local |
| O‘qituvchi | teacher@ecohub.local |

O‘quvchi demo akkaunti:

- Login: `student001@ecohub.local`
- Parol: `Student123!`

Loyiha birinchi ishga tushganda 10 ta sinf va 300 ta namunaviy o‘quvchi avtomatik yaratiladi.

## 4. Papkalar

- `frontend/` — brauzer interfeysi.
- `backend/` — Express server, API, controller va middleware.
- `database/schema.sql` — SQL jadvallari.
- `database/ecohub.sqlite` — birinchi ishga tushishda avtomatik yaratiladigan SQLite bazasi.

## 5. Muhim eslatma

Bu lokal ishlab chiqish uchun tayyorlangan MVP. Internetga chiqarishdan oldin:
- `.env` ichidagi `SESSION_SECRET` qiymatini kuchli maxfiy qiymatga almashtiring.
- Demo akkauntlar parollarini almashtiring.
- HTTPS va production uchun mos session store sozlang.
- Maktabning haqiqiy shaxsiy ma’lumotlarini demo muhitga joylamang.

# SQL_Odev2
lcw bootcamp sql 2.ödev reposudur.

-- 1. Film Tablosunda bulunan tüm sütunlardaki verileri replacement_cost değeri 12.99'dan büyük eşit ve 16.99'dan küçük olma koşuluyla sıralama (BETWEEN - AND kullanarak)
SELECT *
FROM film
WHERE replacement_cost BETWEEN 12.99 AND 16.99
ORDER BY title;

-- 2. Actor Tablosunda bulunan first_name ve last_name sütunlarındaki verileri, first_name 'Penelope', 'Nick' veya 'Ed' olması koşuluyla sıralama (IN operatörünü kullanarak)
SELECT first_name, last_name
FROM actor
WHERE first_name IN ('Penelope', 'Nick', 'Ed')
ORDER BY first_name;

-- 3. Film Tablosunda bulunan tüm sütunlardaki verileri, rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşuluyla sıralama (IN operatörünü kullanarak)
SELECT *
FROM film
WHERE rental_rate IN (0.99, 2.99, 4.99)
  AND replacement_cost IN (12.99, 15.99, 28.99)
ORDER BY title;


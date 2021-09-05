# SQL_ODEV3
**Patika SQL eğitimi kapsamındaki ödev3**
1._country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız._
```sql
SELECT country FROM country WHERE country LIKE 'A%a';
```
2._country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız._
```sql 
SELECT country FROM country WHERE country LIKE '_____%n';
```
3._film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız._
```sql
SELECT title FROM film WHERE title ILIKE 'T%T%T%T%';
```
4._film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız._
```sql
SELECT * FROM film WHERE title LIKE 'C%' AND length>90 AND  rental_rate = 2.99
```

Sorgu senaryolarını [dvdrental.tar](https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip) isimli dosyayı indirerek gerçekleştirebilirsiniz.

# dvdrental_odev11
patika.dev veri tabanı işlemleri ödev11

1) actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.
```
(SELECT first_name FROM actor)
UNION ALL
(SELECT first_name FROM customer);
```
![1](sorgu_1.jpg)
***
2) actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.
```
(SELECT first_name FROM actor)
INTERSECT
(SELECT first_name FROM customer);
```
![2](sorgu_2.jpg)
***
3) actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
```
(SELECT first_name FROM actor)
EXCEPT
(SELECT first_name FROM customer);
```
![3](sorgu_3.jpg)

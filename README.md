# sql_odev_8
SQL 8. Ödevi

1. *test* veritabanınızda *employee* isimli sütun bilgileri *id*(INTEGER), *name* VARCHAR(50), *birthday* DATE, *email* VARCHAR(100) olan bir tablo oluşturalım.

```SQL
      CREATE TABLE employee(
	    id INT,
	    name VARCHAR(50),
	    birthday DATE,
    	email VARCHAR(100)
      );
```

***

2. Oluşturduğumuz *employee* tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```SQL
      insert into employee (id, name, birthday, email) values (1, 'Jacquenetta', '1959-08-16', 'jjervis0@wisc.edu');
      insert into employee (id, name, birthday, email) values (2, 'Gottfried', '1952-06-04', 'gcoast1@redcross.org');
      insert into employee (id, name, birthday, email) values (3, 'Samaria', '1981-02-07', 'sglasman2@ucsd.edu');
      insert into employee (id, name, birthday, email) values (4, 'Cristionna', '1946-08-22', 'cnewall3@ameblo.jp');
      insert into employee (id, name, birthday, email) values (5, 'Oliy', '1942-02-13', 'omartignon4@hubpages.com');
      ...
```

***

3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

```SQL
      UPDATE employee SET name = 'Ali', birthday = '2000-01-01', email = 'ali@veli.com' WHERE id = 10;
      UPDATE employee SET name = 'Hıdır', birthday = '1990-01-01', email = 'hidir@dir.com' WHERE id = 15;
      UPDATE employee SET name = 'Kahraman', birthday = '1923-01-01', email = 'kahraman@celal.com' WHERE id = 20;
      UPDATE employee SET name = 'Nihal', birthday = '1995-01-01', email = 'nihal@demir.com' WHERE id = 25;
      UPDATE employee SET name = 'Kerem', birthday = '1998-01-01', email = 'kerem@gok.com' WHERE id = 30;
```

***

4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

```SQL
      DELETE FROM employee WHERE name = 'Ali';
      DELETE FROM employee WHERE name = 'Hıdır';
      DELETE FROM employee WHERE name = 'Kahraman';
      DELETE FROM employee WHERE name = 'Nihal';
      DELETE FROM employee WHERE name = 'Kerem';
```

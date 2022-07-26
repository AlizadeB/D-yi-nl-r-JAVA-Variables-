# Dəyişənlər (JAVA Variables)

![Uygulama Ekran Görüntüsü](https://miro.medium.com/max/875/1*Px7h03Ih7B5QZu4KQpSEoQ.png)

**Şəkil 1.** Verilənlər (dəyərlər : 4, 2.5, “a”, “hello”) və dəyişənlər (myInt, myReal, myChar, myString)

-	Dəyişən proqramının icrası zamanı dəyəri özündə saxlayan məlumat qutusudur. 
-	Hər bir dəyişənin tipi vardır. Bu tip həmçinin qutuda tutulacaq məlumatın miqdarını təyin edir.
-	Dəyişən verilənlər üçün yaddaş yeri adıdır. Məsələn: biz 4500 dəyərini maaş qutusuna daxil edirik. 4500 dəyərinin yaddaş yerindəki adı maaşdır.

## Bəs niyə məhz dəyişən adlandırılır?

-	Dəyişəndə saxlanılan dəyər proqramın icrası zamanı dəyişdirilə bilər.
-	Dəyişən yalnız ünvandır. Dəyişən üzərində edilən bütün əməliyyatlar həmin yaddaş yerinə təsir edir.
-	Java-da bütün dəyişənlər istifadə edilməzdən əvvəl elan edilməlidir, yəni dəyər verib sonra dəyişən verə bilmərik.

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/a1a9fea2b739d6650f1a4ca966c5c072.png)

! Nümunədəki `“=”` işarəsi `mənimsətmə operatorudur`, `bərabərlik deyil`. Həmçinin `int` bir `tipdir`. Bu haqda Operatorlar və Verilən tipləri mövzusunda ətraflı məlumat veriləcək.

Dəyişən qeyd etdiyimiz kimi tipə malik olmalıdır. Bu bir insanın müəyyən bir xüsusiyyətə malik olması kimidir. Məsələn: Turanə çalışqan bir tələbədir. `Tələbə` mənim `dəyişənim`, `Turanə` `verilən dəyər`, `çalışqan` da `tipdir`. Verilən tipləri haqqında bir sonrakı mövzuda danışacağıq. 

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/f601d6da863bdd1c113ea70fcca7b6e1.png)

## Dəyişənlə bağlı vacib nüanslar

- Dəyişən verilənlə bərabər təyin edilə bilər.
-	Eyni anda bir tip ilə birdən çox dəyişən təyin edilə bilər.
-	Dəyişən təyin edildikdən sonra da verilən mənimsədilə bilər.
-	Dəyişənin dəyəri ən son mənimsədiləndir.
-	Hətta dəyişən bir başqa dəyişənə də mənimsədilə bilər.

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/3109e8d8ae32fd0bfb378d50e9358fb8.png)

## Dəyişənin növləri:
-	#### Yerli/lokal dəyişənlər (Local Variables)
-	####	Müraciət/nümunə dəyişənlər (Instance Variables)
-	####	Statik dəyişənlər (Static Variables)

Dəyişənlər işlənmə yerinə görə müxtəliflik təşkil edir. Gəlin nümunə üzərindən izah edək: 
-	Sinifdə Java proqramlaşdırma dilindən istifadə olunur və burada keçilənlər sadəcə bu sinif daxilində bilinir. Sinifdən kənar şəxslər bu məlumata malik deyillər. Bu `lokal dəyişəni` təmsil edir.
-	Tələbə transkript almaq istəyirsə universitet daxilində müvafiq dekanlığa müraciət edib bu sənədi əldə edə bilər. Bu `müraciət dəyişənini` ifadə edir.
-	Tələbənin tələbə bileti universitet daxilində hər bir yerdə keçərlidir. Heç bir müraciətə ehtiyac yoxdur. Bu da `statik dəyişəndir`.

### Yerli/lokal dəyişənlər
-	Yerli dəyişənlər metodlarda, konstruktorlarda və ya bloklarda elan edilir. 
-	Metod, konstruktor və ya blok daxil edildikdə yerli dəyişənlər yaradılır.
-	Dəyişən metoddan, konstruktordan və ya blokdan çıxdıqdan sonra məhv edilir və artıq istifadə edilə bilmir.

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/828eed9e5c0eb904d167305d900088da.png)

### Müraciət/nümunə dəyişənlər
- Sinif daxilində olan bu dəyişənlər metod, konstruktor xaricində elan edilən dəyişənlərdir.
- Bu dəyişənlər dəyişənin çoxlu istifadəsini asanlaşdırır.
- Sinfin referans dəyişəni vasitəsilə müraciət edilərək çağırılır.

Aşağıdakı nümunədə **psvm**-dən (`ipublic static void main` – bu bir qısa açarla ifadə olunmuş **metoddur**) kənar transkript dəyişəni yaradılıb. Qarşısında **tipi** və **spesifikatoru** verilib. Bu haqda spesifikatorlar mövzusunda danışacağıq. Daha sonra psvm daxilində əvvəlcə **sinfin referans dəyişəni** elan edilib (`Numune numune = new Numune();`)  Bu haqda isə Sinif, obyekt, konstruktor və metodlar mövzusunda ətraflı öyrənəcəyik. Daha sonra isə dəyişən müraciət edilərək çağırılıb. Bəzəkli mötərizələr **{ }** bizə hüdudları bildirir.

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/cad2b5fdbfa4e0287c199d0a804c6f31.png)

Aşağıdakı nümunədə əvvəlcə boş şəkildə dəyişən elan edilib daha sonra konstruktor daxilində 
**this** açar sözü ilə çağırılaraq dəyər mənimsədilib. Sonra isə eyni dəyişən metod daxilində referans dəyişəni elan edilərək çağırılıb sonda isə ekrana nəticə şəklində verilib.

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/aa5901378f3c7f52453c64652e5c0d6a.png)

### Statik dəyişənlər
-	Statik dəyişənlərin müraciət dəyişənlərindən əsas fərqi **static** açar sözündən istifadə olunmasıdır. Bu sayədə sinfin referans dəyişəni elan edilmədən birbaşa sinif adı ilə çağırmanı təmin edir. 

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/b75835b68030762b6291db8de589b281.png)

**Aşağıdakı nümunədə hər üç dəyişən növü birgə işlənmişdir:**

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/7f57dcf64174266be14f0ad7fc994011.png)


## İstinadlar

Bu yazı aşağıdaki mənbələrdən yararlanılaraq hazırlanmışdır:

- https://www.tutorialspoint.com/What-are-class-variables-instance-variables-and-local-variables-in-Java
- https://www.geeksforgeeks.org/variables-in-java/

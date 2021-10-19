# Kodluyoruz Insertion Sort Projesi
```
A) [22,27,16,2,18,6] -> Insertion Sort

1.	Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2.	Big-O gösterimini yazınız.
3.	Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4.	Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
```
> Çözüm A:    [22,27,16,2,18,6]
1.	[2,27,16,22,18,6]          en küçük 2 olduğu için 22 ve 2 yer değiştirdi 

    [2|6,16,22,18,27]  kalan en küçük 6 olduğu için 27 ve 6 yer değiştirdi

    [2,6|16,22,18,27] 16 en küçük sayı oldugu için dizi değişmedi

    [2,6,16|18,22,27] kalan en küçük 18 olduğu için 22 ve 18 yer değiştirdi

    [2,6,16,18|22,27]         kalanlar arasında en küçük 22 oldugu için dizi aynı kaldı

       **->[2,6,16,18,22,27]**

2.	Her adımda bir sayı sıralandığı için sıralanacak geri kalan sayıların sayısı 1 eksilmiş oluyor o halde ardışıl olarak :
  n + (n-1) + (n-2) + ….  + 1   kere işlem yapılır.  n.(n+1) / 2  olarak formülüze edersek işlem sonucu  n²  ‘ li olacak.   Yani O(n²) 

3. Worst case: Aradığımız sayının sonda olması   -> O(n²)

   Average case: Aradığımız sayının ortada olması -> O(n²)   **Algoritmaları analiz ederken, ortalama durum genellikle en kötü durumla aynı karmaşıklığa sahiptir. 

   Best case: Aradığımız sayının dizinin en başında olması. -> O(n)

4.	Dizi sıralandıktan sonra 18 sayısı dizinin ortasında olduğu için Average Case kapsamına girer.

```
 B)  [7,3,5,8,2,9,4,15,6] dizisinin       Insertion Sort'a göre ilk 4 adımını yazınız.
```
> Çözüm B: [7,3,5,8,2,9,4,15,6]

1-> [2,3,5,8,7,9,4,15,6]  en küçük 2 oldugu için 7 ile yer değiştirdi

2-> [2|3,5,8,7,9,4,15,6]  kalan en küçük sayı 3 olduğu için dizi aynı kaldı

3-> [2,3|4,8,7,9,5,15,6] kalan en küçük sayı 4 oldugu için 5 ile yer değiştirdi

4-> [2,3,4|5,7,9,8,15,6] kalan en küçük sayı 5 oldugu için 8 ile yer değiştirdi
 
  **->[2,3,4,5,7,9,8,15,6]**

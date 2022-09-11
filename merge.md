# PROJE 2 

## Merge Sort



## SORU

> [16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.

## CEVAP

[16,21,11,8,12,22]

Dizideki tüm elemanlar, tek eleman kalana dek sağa ve sola doğru ikiye bölünür.

> [16,21,11] [8,12,22]
>>[16,21] [11] [8,12] [22]
>>> [16] [21] [11] [8] [12] [22]

Bu aşamadan sonra tekrar birleşime geçilir.

> [16,21] [11] [8] [12,22]
>>[11,16,21] [8,12,22]
>>> [8,11,12,16,21,22] son birleştirmede dizimizin düzenli son halini elde etmiş oluyoruz.

Time complexity formülü: O(nLogn) şeklindedir. Her ikiye bölünmüş dizinin birleşim (merge) işlemi için dizinin uzunluğu kadar (n kadar) işlem yapılmıştır. O(nLogn) formülü --> O(6(log6)) şeklinde olacaktır.
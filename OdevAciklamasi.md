Dizi: [16,21,11,8,12,22] 

1.Dizinin Merge Sort türüne göre aşamalarını yazınız. 
Burada önce diziyi parçalara bölmemiz ve ardından birleştirmemiz gerekiyor. 

1.Bölme İşlemi: [16,21,11]   --  [8,12,22]


2.Bölme İşlemi: [16,21]-[11]  ----  [8,12]-[22]
Bu şekilde sıralama yapabiliriz. 
[16,21] --> Sıralı bir durumda. Bu küçük dizi parçasında herhangi bir işlem yapmaya gerek yok. 
[11] --> Tek elemanlı oldu. Birleştirirken durumunu göz önüne alacağız. 
[8,12] --> Bu dizide kendi içerisinde küçükten büyüğe sıralanmış durumda. 
[22] --> Tek eleman. Bunu birleştirirken değerlendireceğiz. 

Birleştirme: 
[16,21] + [11] işleminde 11'in, soldaki dizi olan her iki değerden de küçük olduğu görülerek birleştirildiğinde 11 değeri dizinin en başına alınır. 
Birleştirme sonucu yeni mini dizi: [11,16,21] oldu. 

Birleştirme 2: [8,12] + [22] işleminde 22 hepsinden büyük. O nedenle dizinin sonuna yerleşir. 
Birleştirme sonucu yeni mini dizi: [8,12,22] olur. 

Birleştirme 3: [11,16,21] + [8,12,22] 
8 elemanı soldaki dizinin her değerinden küçük. En başa geçer. 
12 elemanı 16'dan küçük. Önüne gelir. 
22, birleştirilen dizi dahil her değerden küçük. Yerinde kalır. 

Bu sayede yeni dizi: [8,11,16,21,22] olur. 

2.Big-O gösterimini yazınız. 
Merge Sort işleminde dizileri ayırırken O(n) değeri elde edilir. 
Birleştirme aşamasında ise time compl. O(logn)'dir. 

Bu durumda ise genel değer O(nlogn) olur. 

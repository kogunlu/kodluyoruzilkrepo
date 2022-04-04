# Merge Sort Projesi

## Proje 2
[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
--- 
## Yanıtlar
### 1. Sorunun Yanıtı
1. Dizinin boyutu 6 olduğu için mid elemanı 2. indisteki **11**'e karşılık gelir.
2. Dizimizi ortadaki sayının sağı ve solu olacak şekilde ikiye böleriz;
    - elimizde [16,21,11] ve [8,12,22] olarak iki parça oluşur. 
3. Dizideki elemanlar tek kalıncaya kadar her seferinde 2 ye bölmeye devam ederiz;

    - [16,21] ve [11] sol tarafta    ||||||||||   [8,12]  ve [22] sağ tarafta kalır 
    - [16] [21]  [11]          ||||||||          [8] [12] [22]
 4. Tüm elemanlar tek başına kalınca karşılaştırıp sıralı bir şekilde birleştiririz;
    - [16,21] ve [11]  sol tarafta     |||||||||   [8,12] ve [22] sağ tarafta  
    - [11,16,21] sol tarafta   |||||||||  [8,12,22] sağ tarafta
 6. İki dizinin en sol üyülerinden başlayarak karşılaştırma yapılır ve birleştirilir.
    - [8,11,12,16,21,22]  

**### Görsel olarak göstermek gerekirse;**

    [16, 21, 11, 8, 12, 22]
        /             \
    [16, 21, 11]     [8, 12, 22]
      /   \           /   \
    [16, 21] [11]   [8, 12] [22]
      /  \     |      /  \    |
    [16] [21]  [11]  [8] [12] [22]
      \       /       \      /    
    [11, 16, 21]    [8, 12, 22]
          \             /
    [8, 11, 12, 16, 21, 22]


### 2. Sorunun Yanıtı
 - O(nlogn)


    





         
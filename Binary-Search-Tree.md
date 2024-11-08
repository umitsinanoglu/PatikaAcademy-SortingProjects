# Proje 3 - Binary Search Tree Ağaç Yapısı

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

#### Adım 1: İlk Eleman (7)
İlk eleman olan **7**, ağacın kökü (root) olur.
```
    7
```

#### Adım 2: 5
**5**, **7**'den küçük olduğu için **7**'nin soluna eklenir.
```
    7
   /
  5
```

#### Adım 3: 1
**1**, **7**'den ve **5**'ten küçük olduğu için **5**'in soluna eklenir.
```
    7
   /
  5
 /
1
```

#### Adım 4: 8
**8**, **7**'den büyük olduğu için **7**'nin sağına eklenir.
```
    7
   / \
  5   8
 /
1
```

#### Adım 5: 3
**3**, **7**'den küçük, ancak **5**'ten büyük olduğu için **5**'in sağında yer alır.
```
    7
   / \
  5   8
 / \
1   3
```

#### Adım 6: 6
**6**, **7**'den küçük, ancak **5**'ten büyük olduğu için **5**'in sağında, **3**'ten büyük olduğu için **3**'ün sağında yer alır.
```
    7
   / \
  5   8
 / \
1   3
     \
      6
```

#### Adım 7: 0
**0**, **7**, **5** ve **1**'den küçük olduğu için **1**'in soluna eklenir.
```
    7
   / \
  5   8
 / \
1   3
/     \
0       6
```

#### Adım 8: 9
**9**, **7** ve **8**'den büyük olduğu için **8**'in sağına eklenir.
```
    7
   / \
  5   8
 / \    \
1   3    9
/     \
0       6
```

#### Adım 9: 4
**4**, **7** ve **5**'ten küçük, ancak **1** ve **3**'ten büyük olduğu için **3**'ün sağında, **6**'dan küçük olduğu için **6**'nın solunda yer alır.
```
    7
   / \
  5   8
 / \    \
1   3    9
/     \
0       6
       /
      4
```

#### Adım 10: 2
**2**, **7** ve **5**'ten küçük, ancak **1**'den büyük, **3**'ten küçük olduğu için **3**'ün soluna, **4**'ten küçük olduğu için **4**'ün soluna eklenir.
```
    7
   / \
  5   8
 / \    \
1   3    9
/     \
0       6
     /   \
    4     2
```

### Sonuç: Tamamlanmış Binary Search Tree

```
        7
       / \
      5   8
     / \    \
    1   3    9
   /     \
  0       6
         /   \
        4     2
```

Bu ağaç yapısında:
- **Root (Kök):** 7
- **Sol Yarı (Left Subtree):** 5, 1, 3, 0, 6, 4, 2
- **Sağ Yarı (Right Subtree):** 8, 9

Her bir eleman, Binary Search Tree kurallarına uygun olarak karşılaştırmalarla doğru konumda yerleştirilmiştir.

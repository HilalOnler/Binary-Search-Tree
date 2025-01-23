# **BINARY SEARCH TREE PROJESİ**


**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]**  dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

---



## ***Binary Search Tree (BST) Adımları***

Binary Search Tree (BST), her düğüm için "solundaki düğümler küçük, sağındaki düğümler büyük" olacak şekilde bir ağaç oluşturur.

**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]** -> Başlangıç
1.   İlk eleman **root** olur:
```
Root: 7
```
2.   5 eklenir:
5, 7'den küçük olduğu için **soluna** eklenir.
```
            7
           /
          5
```
3.   1 eklenir:
1, 7'den küçük, 5'ten de küçük olduğu için 5'in **soluna** eklenir.
```
            7
           /
          5
         /
        1
```
4.   8 eklenir:
8, 7'den büyük olduğu için 7'nin **sağına** eklenir.
```
            7
           / \
          5   8
         /
        1
```
5.   3 eklenir:
3, 7'den ve 5'den küçük ancak 1'den büyük olduğu için 1'in **sağına** eklenir.
```
            7
           / \
          5   8
         /
        1
         \
          3
```
6.   6 eklenir:
6, 7'den küçük ancak 5'den büyük olduğu için 5'in **sağına** eklenir.
```
            7
           / \
          5   8
         / \
        1   6
         \
          3
```
7.   0 eklenir:
0, 7'den, 5'den ve 1'den küçük olduğu için 1'in **soluna** eklenir.
```
            7
           / \
          5   8
         / \
        1   6
       / \
      0   3
```
8.   9 eklenir:
9, 7'den ve 8'den büyük olduğu için 8'in **sağına** eklenir.  
```
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
```
9.   4 eklenir:
4, 7'den ve 5'den küçük, 1'den ve 3'den büyük olduğu için 3'ün **sağına** eklenir.  
```
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
           \
            4
```
10.  2 eklenir:
2, 7'den ve 5'den küçük, 1'den büyük ancak 3'den küçük olduğu için 3'ün **soluna** eklenir.  
```
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
         / \
        2   4
```

## ***Dizinin Son Hali***
*[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]*
```
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
         / \
        2   4
```
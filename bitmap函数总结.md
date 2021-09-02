```
clickhouse bitmap函数：
1、bitmapBuild(array) 构造bitmap
2、bitmapToArray  将bitmap转成整型array
3、bitmapContains(bitmap, e)   判断指定bitmap中是否存在e元素
4、bitmapHasAny(bitmap1, bitmap2)  bitmap1中是否包含bitmap2中的元素，只要有一个相同的元素，就返回1，否则返回0.
5、bitmapHasAll(bitmap,bitmap) bitmap1中是否全部包含bitmap2中的元素，全部包含就返回1，否则返回0.
6、bitmapCardinality(bitmap) 返回bitmap的基数
7、bitmapAnd(bitmap,bitmap) 求两个bitmap的交集
8、bitmapOr(bitmap,bitmap) 求两个bitmap的并集
9、bitmapXor(bitmap,bitmap) 求两个bitmap的异或
10、bitmapAndnot(bitmap1,bitmap2) 求bitmap1与bitmap2的与非
11、bitmapSubsetInRange(bitmap, range_start, range_end)
返回bitmap中，range_start到range_end区间内（不包含renge_end）的子集bitmap对象
12、bitmapSubsetLimit(bitmap, range_start, cardinality_limit)
返回bitmap中，从range_start开始的cardinality_limit个元素组成的子集bitmap对象
```

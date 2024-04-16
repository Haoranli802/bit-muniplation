# bit-muniplation
## 位运算类问题

***

JZ15二进制中1的数量

```
public int NumberOf1 (int n) {
    // write code here
    int res = 0;
    while(n != 0){
        n &= n - 1;
        res++;
    }
    return res;
}
```
n & n-1 可以让二进制数字中最后一个1变为0而其他不变，我们可以一直做n & n-1知道n变成0这样就能找到n中有多少个1

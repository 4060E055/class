# <一>getchar(字元) & putchar(字元) 函数

```
讀取一個單一的字元
p.s:不受存取變數型態的影響
```
```
#include <stdio.h>//在stdio標頭檔裡
int main( )
{
   int c;
   printf( "Enter a value :");
   c = getchar( );//讀取一個字元
   printf( "\nYou entered: ");
   putchar( c );//輸出一個字元
   printf( "\n");
   return 0;
}
```

# <二>gets(字串) & puts(字串) 函数
```
讀取一串字串
p.s:字元陣列多於沒用到的空間依然會佔存取，使用指標陣列不會
```
```
#include <stdio.h>//在stdio標頭檔裡
int main( )
{
   char str[100];//宣告一個字元陣列
 
   printf( "Enter a value :");
   gets( str );//把輸入的字串分別丟到字元陣列裡面
 
   printf( "\nYou entered: ");
   puts( str );//輸出該陣列
   return 0;
}
```

# <三>scanf(型態,位址) 和 printf(型態,變數) 函数
```
型態有：%d(整數),%ld(長整數),%f(浮點數),%lf(背精度浮點數),%c(字元),%s(字串)
p.s:變數前面+ "&" 可變成變數的位址
```
```
#include <stdio.h>
int main( ) {
 
   char str[100];
   int i;
 
   printf( "Enter a value :");
   scanf("%s %d", str, &i);//讀取字串跟整數，&i為i的位址
 
   printf( "\nYou entered: %s %d ", str, i);
   printf("\n");
   return 0;
}
```
```

```
上傳圖片
![result](相對路徑)





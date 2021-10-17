```Java
System.out.println("hello world");
```

    hello world
    


```Java
int add(int a, int b)
{
    return a + b;
}
```


```Java

```


```Java
add(2, 3)
```




    5




```Java
void brush()
{
    System.out.println("yagk");
    System.out.println("uwya");
}
```


```Java
brush()
```

    yagk
    uwya
    

## 方法的定义 method

* 函数的返回值类型
* 空格
* 方法名称
* 括号
* 参数，放到方法名称后面的括号中，表示方法执行需要的信息


```Java
void dance() // 只做事情
{
    System.out.println("you can really dance");
}
```


```Java
dance()
```

    you can really dance
    


```Java
void complex()
{
    brush();
    dance();
}
```


```Java
complex()
```

    yagk
    uwya
    you can really dance
    


```Java
// expression
1 * 2
```




    2




```Java
int a = 2 * 3 + 4;
```


```Java
a * 2
```




    20




```Java
int add(int a, int b) // parameter, placeholder,
{
    return a + b;
}
```


```Java
add(2, 3)
```




    5




```Java
void void_add(int a, int b)
{
    System.out.print(a + b);
}
```


```Java
void_add(2, 3)
```

    5


```Java
void_add(2, 3) * 5
```


    |   void_add(2, 3) * 5

    此处不允许使用 '空' 类型

    



```Java
add(2, 3) * 5
```




    25




```Java
add(add(2, 3), add(1, 4))
```




    10



## override 重载


```Java
String add(String s1, String s2) // 返回值的类型是字符串 String
{
    // System.out.println(s1 + s2);
    return s1 + s2;
}
```


```Java
add("hello ", "world");
```




    hello world




```Java
1 // evalution
```




    1




```Java
void count(int n)
{
    System.out.println(n);
    if(n != 1)
    {
        count(n-1);
    }
}
```


```Java
count(1);
System.out.println("end");
```

    1
    end
    


```Java
count(2)
```

    2
    1
    


```Java
count(3)
```

    3
    2
    1
    


```Java
void bingbao(int n)
{
    System.out.print(n + " ");
    if(n != 1)
    {
        if(n % 2 == 0)
        {
            bingbao(n/2);
        }
        else
        {
            bingbao(3*n+1);
        }
    }
}
```


```Java
bingbao(1)
```

    1 


```Java
bingbao(2)
```

    2 1 


```Java
bingbao(3)
```

    3 10 5 16 8 4 2 1 


```Java
int total(int n)
{
    if(n == 1)
    {
        return 1;
    }
    else
    {
        return n + total(n-1);
    }
}
```


```Java
total(1)
```




    1




```Java
total(2)
```




    3




```Java
total(3)
```


```Java

```

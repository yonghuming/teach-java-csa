## 迭代


```Java
public static void greet()
{
    System.out.print("挤牙膏 ");
    System.out.print("刷牙 ");
    System.out.print("清洗 ");
}
```


```Java
greet();
```

    挤牙膏 刷牙 清洗 


```Java
void greet2()
{
    greet();
    greet();
}
```


```Java
greet2()
```

    挤牙膏 刷牙 清洗 挤牙膏 刷牙 清洗 


```Java
void count(int n)
{
    System.out.print(n + " ");
    if(n > 1)
    {
        count(n-1);
    }
}
```


```Java
count(1)
```

    1 


```Java
count(2)
```

    2 1 


```Java
1 + " " + 2
```




    1 2




```Java
count(3)
```

    3 2 1 


```Java
void bingbao(int n) // void method
{
    System.out.print(n + " ");
    if(n != 1)
    { // code block
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
bingbao(1);
System.out.println("done");
```

    1 done
    


```Java
bingbao(2)
```

    2 1 


```Java
bingbao(2) * 2
```


    |   bingbao(2) * 2

    此处不允许使用 '空' 类型

    



```Java
bingbao(3)
```

    3 10 5 16 8 4 2 1 


```Java
bingbao(7)
```

    7 22 11 34 17 52 26 13 40 20 10 5 16 8 4 2 1 


```Java
int add(int n) // value mehtod
{
    return n;
}
```


```Java
add(1) * 3
```




    3




```Java
int add(int n)
{
    System.out.print(n + " ");
    if(n > 1)
    {
        return n + add(n-1);
    }
    else
    {
        return 1;
    }
}
```


```Java
add(1)
```

    1 




    1




```Java
add(2)
```

    2 1 




    3




```Java
add(3)
```

    3 2 1 




    6




```Java
add(4)
```

    4 3 2 1 




    10




```Java
int add(int n)
{
    System.out.print(n + " ");
    if(n > 1)
    {
        return n + add(n-2);
    }
    else
    {
        return 1;
    }
}
```


```Java
add(5)
```

    5 3 1 




    9



## while
循环，初始值，最终值和步长。


```Java
int counter = 0;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    System.out.print(counter + " ");
    counter += 1; // counter = counter + 1
}
```

    0 1 2 3 4 5 6 7 8 9 


```Java
int counter = 0;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    counter += 1; // counter = counter + 1
    System.out.print(counter + " ");
}
```

    1 2 3 4 5 6 7 8 9 10 


```Java
int n = 2;
while(n != 1)
{
    System.out.print(n + " ");
    if(n % 2 == 0) // % 取余数 n 除以 2 的余数
    {
        n = n / 2;
    }
    else
    {
        n = 3 * n + 1;
    }
}
System.out.print(n + " end");
```

    2 1 end


```Java
int n = 3;
while(n != 1)
{
    System.out.print(n + " ");
    if(n % 2 == 0)
    {
        n = n / 2;
    }
    else
    {
        n = 3 * n + 1;
    }
}
System.out.println("");
System.out.println(n + " end");
```

    3 10 5 16 8 4 2 
    1 end
    


```Java
int counter = 0;
int total = 0;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    counter += 1; // counter = counter + 1
    total = total + counter;
    System.out.print(total + " ");
}
System.out.println("");
System.out.print(total + " end");
```

    1 3 6 10 15 21 28 36 45 55 
    55 end


```Java
int counter = 0;
int production = 1;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    counter += 1; // counter = counter + 1
    production = production * counter;
    System.out.print(production + " ");
}
System.out.println("");
System.out.print(production + " end");
```

    1 2 6 24 120 720 5040 40320 362880 3628800 
    3628800 end


```Java
int counter = 1;
int production = 1;
while(counter < 11) // 如果这个表达式成立，就执行后面的代码块
{
    production = production * counter;
    counter += 1; // counter = counter + 1
    System.out.print(production + " ");
}
System.out.println("");
System.out.print(production + " end");
```

    1 2 6 24 120 720 5040 40320 362880 3628800 
    3628800 end


```Java
int counter = 0;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    if(counter % 2 == 0) // % 取余数
    {
        System.out.print(counter + " ");
    }
    counter += 1; // counter = counter + 1
}
```

    0 2 4 6 8 


```Java
int counter = 0;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    if(counter % 2 == 1) // % 取余数
    {
        System.out.print(counter + " ");
    }
    counter += 1; // counter = counter + 1
}
```

    1 3 5 7 9 


```Java
int counter = 1;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    if(counter % 2 == 0) // % 取余数
    {
        System.out.print(counter + " ");
    }
    counter += 1; // counter = counter + 1
}
```

    2 4 6 8 


```Java
int counter = 1;
while(counter < 10) // 如果这个表达式成立，就执行后面的代码块
{
    System.out.print(counter + "==");
    if(counter % 2 == 0) // % 取余数
    {
        System.out.print(counter + " ");
    }
    counter += 2; // counter = counter + 1 step 步长
}
```

    1==3==5==7==9==

## for 循环


```Java
for(int number = 10; number > 0; number--)
{
    System.out.print(number + " ");
} // zero
```

    10 9 8 7 6 5 4 3 2 1 


```Java
int number = 10;
while(number > 0)
{
    System.out.print(number + " ");
    number = number - 1;
}
```

    10 9 8 7 6 5 4 3 2 1 


```Java

```

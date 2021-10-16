## function

```
def add(a, b):
    return a + b
```


```Java
System.out.println("hello");
```

    hello
    


```Java
System.out.println("word");
```

    word
    


```Java
void greet() 
{
    System.out.println("hello");
    System.out.println("word");
}
```


```Java
greet()
```

    hello
    word
    


```Java
int add(int n1, int n2) // function or mehtod signature, return type: int, space ,
//method name:int, parameter: n1 && n2
{
    return n1 + n2; // value method 值方法 
}
```


```Java
add(2, 3)
```




    5




```Java
add(2, 3) / 2 
```




    2




```Java
void void_add(int n1, int n2) // function or mehtod signature, return type: int, space ,
//method name:int, parameter: n1 && n2
{
    System.out.println(n1 + n2);
} // 2, 3, true, String
```


```Java
void_add(2, 3) 
```

    5
    


```Java
void_add(2, 3) / 2
```


    |   void_add(2, 3) / 2

    此处不允许使用 '空' 类型

    



```Java
add(add(2, 3), 5)
```




    10




```Java
add(2, 3) * 7
```




    35




```Java
void_add(2, 3) * 2
```


    |   void_add(2, 3) * 2

    此处不允许使用 '空' 类型

    



```Java
void_add(void_add(2, 3), 2)
```


    |   void_add(void_add(2, 3), 2)

    此处不允许使用 '空' 类型

    



```Java
void print(String s)
{
    System.out.println(s);
}
```


```Java
print("hello")
```

    hello
    


```Java
void hello(String s) // void function
{
    print(s);
}
```


```Java
hello("hello world")
```

    hello world
    


```Java
Boolean isEven(int num) // method
{
    if(num % 2 == 0)
    {
        return true;
    }
    else
    {
        return false;
    }
}
```


```Java
isEven(2) == false
```




    false




```Java
Boolean flag = true && false || 2 > 3; // expression
```


```Java
flag
```




    false




```Java
Boolean even = isEven(3); // method
```


```Java
even
```




    false




```Java
Boolean isOdd(int num)
{
    if(num % 2 == 0)
    {
        return false;
    }
    else
    {
        return true;
    }
}
```


```Java
isOdd(2)
```




    false




```Java
isOdd(3)
```




    true




```Java
"hello " + "world" + " langxm"
```




    hello world langxm




```Java
String con(String s1, String s2)
{
    return s1 + s2;
}
```


```Java
con(con("hello ", "world") , " langxm") // call a metho
```




    hello world langxm




```Java
1 + " hello"
```




    1 hello




```Java
print("hello xpro")
```

    hello xpro
    


```Java
print(1)
```


    |   print(1)

    不兼容的类型: int无法转换为java.lang.String

    



```Java
print(true)
```


    |   print(true)

    不兼容的类型: boolean无法转换为java.lang.String

    


## 重载
方法重载


```Java
// override 重载
void print(int s)
{
    System.out.println(s);
}
```


```Java
print(1)
```

    1
    


```Java
// override 重载
void print(Boolean s) // parameter just like a placeholder
{
    System.out.println(s);
}
```


```Java
print(true)
```

    true
    


```Java
void print(Boolean b, int n)
{
    System.out.println(b + ", " + n);
}
```


```Java
print(2 > 3 && 5 < 4, 1)
```

    false, 1
    


```Java
void print(String s, int n)
{
    System.out.println(s + ", " + n);
}
```


```Java
print("hello", 1)
```

    hello, 1
    


```Java
void print(int n, String s)
{
    System.out.println(s + ", " + n);
}
```


```Java
print(1, "hello")
```

    hello, 1
    


```Java
// w, h, area
int w = 2;
int h = 3;
int area = w * h;
```


```Java
// function return rectangle's area with width w and height h
```


```Java
int area(int w, int h)
{
    return w * h;
}
```


```Java
area(2, 3)
```




    6




```Java
int perimeter(int w, int h)
{
    return 2 * (w + h);
}
```


```Java
perimeter(2, 3)
```




    10




```Java
// fence $10 per mether
// grass $100 per square mether
```


```Java
int w = 10;
int h = 2;
// 20 * 100 + 24 * 10
10 * perimeter(w, h)
```




    240




```Java
100 * area(w, h)
```




    2000




```Java
10 * perimeter(w, h) + 100 * area(w, h)
```




    2240




```Java
int cost(int width, int height, int fence, int grass)
{
    return fence * perimeter(width, height) + grass * area(width, height);
}
```


```Java
int fencePerMeter = 10;
int grassPerMether = 100;
cost(w, h, fencePerMeter, grassPerMether)
```




    2240




```Java
int substract(int a, int b)
{
    return a - b;
}
```


```Java
substract(2, 3)
```




    -1




```Java
// operate type: "+", "-", "*", "/", "%"
// paramater double oprand num1 num2
// return double
```


```Java
double add(double n1, double n2)
{
    return n1 + n2;
}
double sub(double n1, double n2)
{
    return n1 - n2;
}
double multiply(double n1, double n2)
{
    return n1 * n2;
}
double devide(double n1, double n2)
{
    return n1 / n2;
}
double modular(double n1, double n2)
{
    return n1 % n2;
}

```


```Java
double do_operation(String opType, double n1, double n2)
{
    double result = 0.0;
    if(opType == "+")
    {
        result = add(n1, n2);
    }
    else if(opType == "*")
    {
        result = multiply(n1, n2);
    }
    else if(opType == "-")
    {
        result = sub(n1, n2);
    }
    else if(opType == "/")
    {
        result = devide(n1 n2);
    }else if(opType == "%")
    {
        result = modular(n1, n2);
    }
    return result;
}
```


```Java
do_operation("+", 2, 3) == 5
```




    true




```Java
do_operation("*", 2, 3) == 6
```




    false




```Java
do_operation("-", 2, 3) == -1
```




    true




```Java
do_operation("/", 2, 3) == 2.0 / 3
```




    true




```Java
do_operation("%", 2, 3) == 2.0 % 3
```




    true




```Java

```

```Java
// while for loop
// repeate do thing
// for i in range(10)
// list
// for item in list
```


```Java
void print(int i)
{
    System.out.println(i);
}
```


```Java
print(2)
```

    2
    

## 递归


```Java
void count(int n)
{
    print(n);
    if(n > 1){
        count(n - 1); // call method unitl !n > 1
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

    2
    1
    


```Java
count(3)
```

    3
    2
    1
    


```Java
int sum(int n)
{
    if(n > 1)
    {
        return n + sum(n - 1);
    }
    else
    {
        return 1;
    }
}
```


```Java
sum(1)
```




    1




```Java
sum(2)
```

    3
    




    3




```Java
sum(4)
```

    3
    6
    10
    




    10




```Java
sum(5)
```


```Java
void bingbao(int n)
{
    print(n);
    if(n != 1)
    {
        if(n % 2 == 0)
        {
            bingbao(n / 2);
        }
        else
        {
            bingbao(3 * n + 1);
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

    2
    1
    


```Java
bingbao(3)
```

    3
    10
    5
    16
    8
    4
    2
    1
    


```Java
bingbao(7)
```

    7
    22
    11
    34
    17
    52
    26
    13
    40
    20
    10
    5
    16
    8
    4
    2
    1
    

## while 循环


```Java
int counter = 0;
while(counter < 4) // boolean expression, code block
{
    print(counter);
    counter += 1; // counter = counter + 1;
}
```

    0
    1
    2
    3
    


```Java
int counter = 0;
while(counter < 4) // boolean expression, code block
{
    counter += 1; // counter = counter + 1;
    print(counter);
}
```

    1
    2
    3
    4
    


```Java
int n = 7;
while(n != 1)
{
    print(n);
    if(n % 2 == 0)
        {
            n = n / 2;
        }
        else
        {
            n = 3 * n + 1;
        }
}
print(n)
```

    7
    22
    11
    34
    17
    52
    26
    13
    40
    20
    10
    5
    16
    8
    4
    2
    1
    


```Java
int counter = 0;
int sum = 0;
while(counter < 4) // boolean expression, code block
{
    sum += counter; // sum = sum + counter
    counter += 1; // counter = counter + 1;
}
print(sum);
```

    6
    


```Java
int counter = 0;
int sum = 0;
while(counter < 4) // boolean expression, code block
{
    sum *= counter; // sum = sum * counter
    counter += 1; // counter = counter + 1;
}
print(sum);
```

    0
    


```Java
int counter = 0;
int sum = 1;
while(counter < 4) // boolean expression, code block
{
    sum *= counter; // sum = sum * counter
    counter += 1; // counter = counter + 1;
}
print(sum);
```

    0
    


```Java
int counter = 1;
int sum = 1;
while(counter < 4) // boolean expression, code block
{
    sum *= counter; // sum = sum * counter
    counter += 1; // counter = counter + 1;
}
print(sum);
```

    6
    


```Java
int counter = 0; // start, step, end, loop variable
while(counter < 100) // boolean expression, code block
{
    if(counter % 2== 1)
    {
        print(counter);
    }
    counter += 1; // counter = counter + 1;
}
```


```Java
int counter = 1; // start, step, end, loop variable
while(counter < 100) // boolean expression, code block
{
    if(counter % 2== 0)
    {
        print(counter);
    }
    counter += 2; // counter = counter + 1;
}
```


```Java
for(int index = 0; index < 10; index ++)
{
    print(index);
}
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    


```Java
for(int index = 1; index <= 10; index ++)
{
    print(index);
}
```

    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    


```Java

```

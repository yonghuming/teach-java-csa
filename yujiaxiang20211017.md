```Java
"hello".substring(1, 2) // substring 的作用是返回字符串的一部分
```




    e




```Java
"hello".substring(2, 4)
```




    ll




```Java
"world".substring(3, 4)
```




    l




```Java
"xpro".length() // length 方法返回字符串的长度
```




    4




```Java
"java programming".substring(1, "java programming".length())
```




    ava programming




```Java
"hi".length()
```




    2




```Java
String h(String s)
{
    if(s.length()==1)
    {
        return s;
    }
    else
    {
        return h(s.substring(1, s.length())) + s.substring(0, 1);
    }
}
```


```Java
h("langxianmeng")
```




    gnemnaixgnal




```Java
404 / 10 * 10 + 1
```




    401




```Java
int count = 0;
for(int x = 0;x < 4; x++)
{
    for(int y = x; y < 4; y++)
    {
        count ++;
    }
}
count
```




    10



## Software development lifecyclye
### 需求分析
了解需求
### 设计
** 设计界面
** 设计类
需要将问题分解
### coding

## 测试

## 迭代
但是这是个循环


```Java
class Rect
{
    private int width = 0; // 如果不想让类的实例访问属性或者方法，就要定义为 private
    private int height = 0;
    public Rect() // 构造函数
    {
        System.out.println(width + " " + height);
    }
    public Rect(int w) // 构造函数
    {
        width = w;
        System.out.println(width + " " + height);
    }
    public Rect(int w, int h) // 构造函数
    {
        width = w;
        height = h;
        System.out.println(width + " " + height);
    }
    public int getWidth() // accessors
    {
        return width;
    }
    public void setWidth(int w) throws IOException
    {
        if(w == 0)
        {
            // System.out.println("width can not be zero");
            throw new IOException("边长不能为 0");
        }
        else
        {
            width = w;
        }
        
    }
    public int getHeight() // accessors, value method
    {
        return height;
    }
    public void setHeight(int h) throws IOException// void method mutate
    {
        if(h == 0)
        {
            // System.out.println("width can not be zero");
            throw new IOException("边长不能为 0");
        }
        else
        {
            width = h;
        }
    }
    public int perimeter()
    {
        return 2 * (getWidth() + getHeight());
    }
    public int area()
    {
        return getWidth() * getHeight();
    }
    public String toString()
    {
        return "width: " + width + " height: " + height; 
    }
    
}
```


```Java
Rect r = new Rect(); // new 后面调用的是类的构造函数
```

    0 0
    


```Java
r.area()
```




    0




```Java
Rect r2 = new Rect(2); 
```

    2 0
    


```Java
r2.setHeight(0)
```


    ---------------------------------------------------------------------------

    java.io.IOException: 边长不能为 0

    	at Rect.setHeight(#35:46)

    	at .(#164:1)



```Java
Rect r3 = new Rect(2, 3);
```

    2 3
    


```Java
r3.getWidth()
```




    2




```Java
r3.setWidth(10)
```


```Java
r3.getWidth()
```




    10




```Java
r3.setHeight(22)
```


```Java
r3.getHeight()
```




    22




```Java
r3.perimeter()
```




    64




```Java
r3 + " hello"
```




    width: 10 height: 22 hello




```Java
r3
```




    width: 10 height: 22




```Java
System.out.print(r3)
```

    width: 10 height: 22


```Java
Rect r4 = new Rect(2, 5);
// r4.setWidth(0);
r4.setHeight(0);
r4.perimeter();

```

    2 5
    




    4



## 重载
具有相同名字的函数，参数和返回值类型不同。相当于同一个函数可以随机应变。


```Java
int add(int a, int b)
{
    return a + b;
}
```


```Java
add(2, 3)
```




    5




```Java
Boolean add(int a, int b)
{
    return a == b;
}
```


```Java
add(1, 2)
```




    false




```Java
String add(String s1, String s2)
{
    return s1 + s2;
}
```


```Java
add("hell ", "world")
```




    hell world




```Java

```

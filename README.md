- [for循环](#for%e5%be%aa%e7%8e%af)
    - [for循环：](#for%e5%be%aa%e7%8e%af-1)
    - [for循环语法:](#for%e5%be%aa%e7%8e%af%e8%af%ad%e6%b3%95)
    - [快捷键100.for然后ent键快捷输入:](#%e5%bf%ab%e6%8d%b7%e9%94%ae100for%e7%84%b6%e5%90%8eent%e9%94%ae%e5%bf%ab%e6%8d%b7%e8%be%93%e5%85%a5)
    - [关于for循环有以下几点说明：](#%e5%85%b3%e4%ba%8efor%e5%be%aa%e7%8e%af%e6%9c%89%e4%bb%a5%e4%b8%8b%e5%87%a0%e7%82%b9%e8%af%b4%e6%98%8e)
    - [for的死循环格式：](#for%e7%9a%84%e6%ad%bb%e5%be%aa%e7%8e%af%e6%a0%bc%e5%bc%8f)
    - [for循环的代码示例一（while循环和for循环对比，for死循环示例）：](#for%e5%be%aa%e7%8e%af%e7%9a%84%e4%bb%a3%e7%a0%81%e7%a4%ba%e4%be%8b%e4%b8%80while%e5%be%aa%e7%8e%af%e5%92%8cfor%e5%be%aa%e7%8e%af%e5%af%b9%e6%af%94for%e6%ad%bb%e5%be%aa%e7%8e%af%e7%a4%ba%e4%be%8b)
    - [for循环的代码示例二（练习1：计算0到100之间的奇数和偶数的和,不是偶数和奇数的个数）：](#for%e5%be%aa%e7%8e%af%e7%9a%84%e4%bb%a3%e7%a0%81%e7%a4%ba%e4%be%8b%e4%ba%8c%e7%bb%83%e4%b9%a01%e8%ae%a1%e7%ae%970%e5%88%b0100%e4%b9%8b%e9%97%b4%e7%9a%84%e5%a5%87%e6%95%b0%e5%92%8c%e5%81%b6%e6%95%b0%e7%9a%84%e5%92%8c%e4%b8%8d%e6%98%af%e5%81%b6%e6%95%b0%e5%92%8c%e5%a5%87%e6%95%b0%e7%9a%84%e4%b8%aa%e6%95%b0)
    - [for循环的代码示例三(用while或for循环输出1-1000之间能被5整除的数，并且每行输出3个):](#for%e5%be%aa%e7%8e%af%e7%9a%84%e4%bb%a3%e7%a0%81%e7%a4%ba%e4%be%8b%e4%b8%89%e7%94%a8while%e6%88%96for%e5%be%aa%e7%8e%af%e8%be%93%e5%87%ba1-1000%e4%b9%8b%e9%97%b4%e8%83%bd%e8%a2%ab5%e6%95%b4%e9%99%a4%e7%9a%84%e6%95%b0%e5%b9%b6%e4%b8%94%e6%af%8f%e8%a1%8c%e8%be%93%e5%87%ba3%e4%b8%aa)

### for循环
![](https://img2020.cnblogs.com/blog/1773294/202007/1773294-20200722150948754-51585825.png)

##### for循环：

- 虽然所有循环结构都可以用while或者do…while表示，但Java提供了另一种语句——for循环，使一些循环结构变得更加简单。
- for循环语句是支持迭代的一种通用结构，`是最有效、最灵活的循环机构`。
- for循环执行的次数是在执行前就确定的。语法格式如下：

##### for循环语法:

```java
        for (（初始化;布尔表达式;更新/迭代) {
            //内容 
        }
```



##### 快捷键100.for然后ent键快捷输入:

![](https://img2020.cnblogs.com/blog/1773294/202007/1773294-20200722150936099-1501768434.png)

##### 关于for循环有以下几点说明：

```
/*
关于for循环有以下几点说明：

最先执行初始化步骤。可以声明一种类型，但可初始化一个或多个循环控制变量，也可以是空语句。
然后，检测布尔表达式的值。如架为true，循环体被执行。如果为false，循环终止，开始执行循环体后面的语句。
执行一次循环后，更新循环控制变量（送代因子控制循环变量的增减）。
再次检测布尔表达式。循环执行上面的过程。 
*/
```

##### for的死循环格式：

```java
//死循环
        for (; ; ) {

        }
```

##### for循环的代码示例一（while循环和for循环对比，for死循环示例）：

```java
package com.wenjian.struct;

public class ForDemo01 {
    public static void main(String[] args) {
        int a = 1;           //初始化条件
        while (a <= 100) {   //条件判断
            System.out.println(a);  //循环体
            a += 2;  //迭代
        }
        System.out.println("while语句循环结束");
             //初始化  //条件判断  //迭代
        for (int i = 1; i <= 100; i++) {
            System.out.println(i);
        }
        System.out.println("for循环结束");
        /*
		关于for循环有以下几点说明：
		最先执行初始化步骤。可以声明一种类型，但可初始化一个或多个循环控制变量，也可以是空语句。
		然后，检测布尔表达式的值。如架为true，循环体被执行。如果为false，循环终止，开始执行循环体后面的语句。
		执行一次循环后，更新循环控制变量（送代因子控制循环变量的增减）。
		再次检测布尔表达式。循环执行上面的过程。 
         */

        //死循环
        for (; ; ) {

        }
    }
}

```

##### for循环的代码示例二（练习1：计算0到100之间的奇数和偶数的和,不是偶数和奇数的个数）：

```java
package com.wenjian.struct;

public class ForDemo02 {
    public static void main(String[] args) {
        //练习1：计算0到100之间的奇数和偶数的和,不是偶数和奇数的个数
        int oddsum=0;
        int eventsum=0;

        for (int i = 0; i <= 100; i++) {
            if (i % 2 != 0) {  //奇数
                oddsum = oddsum + i;
            } else {           //偶数
                eventsum = eventsum + i;
            }

        }
        System.out.println("奇数的和" + oddsum);
        System.out.println("偶数的和" + eventsum);
    }
}

输出:

奇数的和2500
偶数的和2550

进程已结束，退出代码 0
```

##### for循环的代码示例三(用while或for循环输出1-1000之间能被5整除的数，并且每行输出3个):


```java
package com.wenjian.struct;

public class ForDemo03 {
    public static void main(String[] args) {
        //练习2：用while或for循环输出1-1000之间能被5整除的数，并且每行输出3个
        for (int i = 0; i <= 1000; i++) {
            if (i % 5 == 0) {
                System.out.print(i+"\t");
            }
            if (i % (5 * 3) == 0) {
                System.out.print("\n");  //println，ln是回车
                //System.out.println();  //或者
            }
        }
                 //println 输出完会换行
         		//print 输出完不会换行
    }
}

输出:
...
965	970	975	
980	985	990	
995	1000	
进程已结束，退出代码 0
```

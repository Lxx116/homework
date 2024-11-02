# **第一周作业**

## ***固定作业***

### **1.本周培训总结**

#### ****嵌入式介绍及学习路线

- **嵌入式系统**：嵌入式系统和硬件设备紧密结合，软件和硬件一起工作，是嵌入到各种设备（如今的各种智能家电等等），控制这些设备工作的一种小型计算机系统。

- **嵌入式的学习路线**：C语言（已初步完成）—>51/STM32（STM32正在往前补充漏看的定时器部分）—>数据结构（队列）—>......—>实时操作系统（RTOS）—>嵌入式Linux

- ##### <u>嵌入式单片机的基本概念*</u：介绍了单片机上一些元件与组成部分以及他们各自的作用。（如下图）

- |   结构   |           **单片机**           |         寄存器         |       最小系统板       |         开发板         |
  | :------: | :----------------------------: | :--------------------: | :--------------------: | :--------------------: |
  | **功能** |   相当于一台微型的电脑寄存器   | cpu内部的数据存储单元  | 只有必要的电路和元器件 | 多一些功能电路和元器件 |
  | **结构** |          **芯片外设**          |        **引脚**        |        **晶振**        |       **复位键**       |
  | **功能** | 芯片封装内的扩展芯片功能的电路 | 片和外部电路通信的接口 |   单片机的外部时钟源   |       重启单片机       |

- **芯片类型的介绍**：STM32F103C8T6 ：入门必备；STM32F103RCT6 ：引脚多，外设多；STM32G431RBT6  ：蓝桥杯的子用这个；STM32H7  ：高性能，可以刷 ；openMV库MSP432/M0：电赛；ESP32 ：物联网；ESP32-CAM：自带摄像头。

- **介绍电路板**（介绍板子：洞洞板与面包板与自己画的板子。立创EDA（初学）Altium Designer（许多企业用））和<u>焊接</u>。

- ##### 运动控制与视觉：<!--这里没有什么很大的印象-->

- **PID算法（闭环控制算法）**：根据系统的输入（给定值）与输出（实际值）之间的偏差，通过<u>比例、积分和微分</u>三个环节进行运算，从而得出控制量来控制被控对象。（调参工具：VOFA+）

- **RTOS（实时操作系统）**：RTOS是一种能够在规定时间内完成特定功能，并对外部事件或数据产生快速响应的操作系统。

  [FreeRTOS的运行原理](https://www.bilibili.com/video/BV1nU411S7We?buvid=XZ2B51225F70B2DA6B9DBF183C95A80229C99&from_spmid=search.search-result.0.0&is_story_h5=false&mid=eQrSLIXlfR8VP8fNLnZ0Mw%3D%3D&plat_id=116&share_from=ugc&share_medium=android&share_plat=android&share_session_id=8b522a9c-20b1-4f55-8612-132aeab76aef&share_source=WEIXIN&share_tag=s_i&spmid=united.player-video-detail.0.0&timestamp=1730003743&unique_k=nzFQa3x&up_id=22082380&share_source=weixin)

- **嵌入式Linux**：Linux是指将Linux操作系统进行修改和优化，以适应嵌入式系统的需求。

  [Linux对应学习教程](https://www.bilibili.com/video/BV1oQ4y1r7To?buvid=XZ2B51225F70B2DA6B9DBF183C95A80229C99&from_spmid=search.search-result.0.0&is_story_h5=false&mid=eQrSLIXlfR8VP8fNLnZ0Mw%3D%3D&plat_id=116&share_from=ugc&share_medium=android&share_plat=android&share_session_id=92ff3a73-373a-47fd-aa7e-772ade0c14c8&share_source=WEIXIN&share_tag=s_i&spmid=united.player-video-detail.0.0&timestamp=1730003818&unique_k=RDJFInl&up_id=42617026&share_source=weixin)

- **QT**：是一个跨平台的应用程序和用户界面开发框架。使用<u>C++编写</u>（后续需要安排学习）。使得开发者能够创建桌面、移动和嵌入式设备上的应用程序。

- **嵌入式高级扩展方向**：机器人（有Robotac赛事，很高级）、嵌入式AI、FPGA（现场可编程门阵列通讯，军工，芯片）、边缘计算设备......

#### Markdown语法

- **使用软件**：使用Typora，或者一些支持markdown的编译器，安装几个插件。

- **功能**：兼容性极强、可读性强、格式转换方便......

- **快捷键**（typora）：1.ctrl+1（2、3、4、5），控制文字的大小，设立标题；

  ​                        2.字体格式的一些CTRL+B：加粗、CTRL+U：下划线、CRTL+T：插入表格等等。<!--这几个我当前笔记较常用-->

  ​                        3.代码块：``` ＋语言＋回车。<!--第一个字符在左上角-->

- **图片插入**：Typora 会先将文件保存到一个固定的目录

- **链接**：ctrl+k，成功后显示蓝色字体

#### **git和github的使用**

[git教程](https://www.bilibili.com/video/BV1s3411g7PS?buvid=XX6BD1D6E6C236F39BA3FD75964D7BE347472&from_spmid=playlist.playlist-detail.0.0&is_story_h5=false&mid=EqyfXsxVREc6B74RZLZ9YQ%3D%3D&plat_id=116&share_from=ugc&share_medium=android&share_plat=android&share_session_id=81da8cc8-d533-4f81-bf14-7d269a175ba4&share_source=WEIXIN&share_tag=s_i&spmid=main.ugc-video-detail.0.0&timestamp=1730009004&unique_k=P0NmSAp&up_id=34786453&share_source=weixin)

- **功能**：版本控制、分支管理、多人协作、备份与恢复、代码分享与开源等等。可以管理代码和提高开发效率

- **使用介绍**：**<!--以下是我的个人实操-->**

  1.安装git

![image-20241029174200557](C:\Users\xx482\AppData\Roaming\Typora\typora-user-images\image-20241029174200557.png)

​       2.创建版本库（）

![image-20241029173921640](C:\Users\xx482\AppData\Roaming\Typora\typora-user-images\image-20241029173921640.png)

![image-20241029173843475](C:\Users\xx482\AppData\Roaming\Typora\typora-user-images\image-20241029173843475.png)

#### c语言补充内容

- **位运算符**：& 与     |或     <<左移      >>右移     ^异或       ~取反

- **bool**：两个取值：<u>true（真）和false（假）</u>，在头文件<stdbool.h>中被定义的

- **extern**：声明变量时<u>多个文件</u>之间共享这些变量

- ##### static：

  1.隐藏：加了 static，就会对其它源文件隐藏，在不同的文件中定义同名函数和同名变量，而不必担心命名冲突。

  2.初始化：存储在静态数据区的变量会在程序刚开始运行时就完成初始化，也是唯一的一次初始化。static变量在函数内部的生命周期是整个程序运行期间，初始化只发生一次

- **define宏定义：**定义常量、变量、宏或函数，增加代码可读性

  ```c
  #define PI 3.14159  
    
  int main() {  
      printf("pi的值为: %f\n", PI);  
      return 0;  
  }
  ```

  输出结果：

  ```c
  pi的值为: 3.141590
  ```

  

- **typedef+结构体**：为结构体取别名

  以下为结构体基本结构(不同初始化)

  ```c
   struct   student //结构体类型 或 结构体名
  {       
   int num;
   char  name[20];     //结构体成员
   char sex;
   int age; 
   float score;
   char addr[30];
   };
  （先定义结构体类型，再定义结构体变量）
   struct student stu1,stu2;       //结构体变量
  ```

  ```c
   struct   data   // 结构体类型 或结构体名
   {      
    int day int month;   //结构体成员
    int year
   }time1,time2;   //结构体变量
  
  ```

  当使用typedef时，不能用第二种初始化方法。

- **typedef+枚举：**使用`enum`关键字定义枚举类型，并指定其名称和列出常量值。

```c
#include <stdio.h>  
  
// 定义一个名为Color的枚举类型 
enum Color {  
    RED,    // 默认情况下，RED的值为0  
    GREEN,  // GREEN的值为1  
    BLUE    // BLUE的值为2  
};  
  
int main() {  
    // 声明一个枚举变量，并将其赋值为GREEN  
    enum Color favoriteColor = GREEN;  
  
    // 使用条件语句来判断favoriteColor的值，并输出对应的结果  
    if (favoriteColor == RED) {  
        printf("你最喜欢的颜色是红色。\n");  
    } else if (favoriteColor == GREEN) {  
        printf("你最喜欢的颜色是绿色\n");  
    } else if (favoriteColor == BLUE) {  
        printf("你最喜欢的颜色是蓝色。\n");  
    }  
  
    return 0;  
}
```

输出结果

```c
你最喜欢的颜色是绿色。
```



### 2.本周自己学习的内容

#### git的学习与了解



#### 定时器

TIM定时中断：初步了解到基本定时器，通用定时器，高级定时器的结构与功能，认识到时基单元（自动重装器、预分频器、计数器）等等。

TIM输出比较：了解到了输出比较（输出一定频率与占空比的PWM）与PWM，还有输出比较模式与相关参数计算

### 3.下周的规划

#### 熟练c语言

每天刷两道编程题（缺乏敲代码经验）<!--尤其是指针函数与函数指针，多熟悉一下-->



## *额外作业*

### void*的特点：

**通用性**：void* 可以指向任何数据类型，这使得它非常灵活。

**类型安全**：使用 void* 会丧失编译器的类型检查，因此程序员需要手动确保类型正确，防止错误。

**强制类型转换**：使用 void* 时，通常需要进行显式的类型转换。

### void*的注意事项：

- 不能对void指针进行算法
- 函数可以接受任意类型的指针，如内存操作函数memcpy与memset

- 普通类型的指针不需要强制转换，直接赋值给void*

### void*实现泛型（个人以链表操作）：

```c
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>  
#include <stdlib.h>  

// 链表节点结构  
typedef struct Node {
    void* data; //指向任意类型数据的指针
    struct Node* next;
} Node;

Node* head=NULL;

// 插入链表
Node* insert(void* data) {
    Node* temp = (Node*)malloc(sizeof(Node));
    temp->data = data;
    temp->next = head;
    head = temp;
    return temp;          // 返回新节点指针
}

// 打印整型数据链表  
void print() {
    Node* temp = head;
    while (temp != NULL) {
        printf("%d ", *((int*)(temp->data)));// 强制转换data指针类型，然后解引用以获取整型数据
        temp = temp->next;
    }
    printf("\n");
}

int main() {
    int num, x;

    printf("有多少数字?\n");
    scanf("%d",&num);
    // 打印链表  

    for (int i = 0; i < num; i++) {
        printf("请输入数字: ");
        scanf("%d", &x);

        // 分配内存存储输入的整型数  
        int* data = (int*)malloc(sizeof(int));
        if (data == NULL) {
            printf("内存分配失败\n");
            exit(1); // 如果内存分配失败，则退出程序  
        }
        *data = x;  

        insert(data); // 将数据的指针插入链表  
        print(); // 打印链表  
    }

    Node* current = head;
    Node* next;
    while (current != NULL) {
        next = current->next;   
        free(current->data);   
        free(current);         
        current = next;      
    }

    return 0;
}
```

### 个人疑问

暂无

### **参考资料**：

[C语言中void*详解及应用- CSDN](https://blog.csdn.net/houzhizhen/article/details/90286984?sharetype=blog&shareId=90286984&sharerefer=APP&sharesource=2401_88101638&sharefrom=link)

[c语言中void *的使用 - CSDN](https://blog.csdn.net/modi000/article/details/104556311?sharetype=blog&shareId=104556311&sharerefer=APP&sharesource=2401_88101638&sharefrom=link)

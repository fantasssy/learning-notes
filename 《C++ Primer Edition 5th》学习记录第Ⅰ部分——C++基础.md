![](https://cdn.nlark.com/yuque/0/2022/png/21578825/1660577849026-1cdff519-d9d2-4b7b-b7f8-59178695745c.png#averageHue=%23ebeae9&clientId=u01061be7-6ca6-4&crop=0&crop=0&crop=1&crop=1&from=paste&id=u9557b22e&margin=%5Bobject%20Object%5D&originHeight=884&originWidth=664&originalType=url&ratio=1&rotation=0&showTitle=false&status=done&style=none&taskId=u3c31ad27-21ad-4103-a6d1-f9810154da7&title=)
<a name="EOXEh"></a>
# 第1章 开始
习题答案见[https://github.com/huangmingchuan/Cpp_Primer_Answers](https://github.com/huangmingchuan/Cpp_Primer_Answers)
<a name="x2MBL"></a>
## 1.2 输入输出
<iostream>库定义如下4个标准IO对象

| cin | 标准输入 |
| --- | --- |
| cout | 标准输出 |
| cerr | 标准错误 |
| clog | 标准日志 |

- 输出运算符<<

左侧是ostream对象，右侧为要输出的内容，**返回值为左侧对象**；输入运算符>>与其类似<br />所以cout<<"Hello World!"<<endl等价于(cout<<"Hello World!")<<endl<br />其中" ... "为字符串常量，std::我已省略<br />标准库对其进行过重载，以适应不同的输入输出值类型

- 控制符endl

首先结束当前行，然后将缓冲区中的东西刷入设备（**刷新流**可以清空缓冲区，避免不必要的错误）

---

**建议调试输出时使用printf，cout如果不刷缓冲区的话不会立即输出！！！**
<a name="c0noQ"></a>
### 练习
<a name="x5PzA"></a>
#### 1.3
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655267804654-4b9ff25f-ee55-4be7-9e34-aa7aef9d6703.png#averageHue=%239abd75&clientId=u9b9a6e72-ffc9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=268&id=u7823020e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=644&originWidth=938&originalType=binary&ratio=1&rotation=0&showTitle=false&size=62530&status=done&style=shadow&taskId=u3a6d4b5f-f3f6-4006-9a01-5e5d51f4a7f&title=&width=389.66668701171875)
<a name="KKYdD"></a>
#### 1.4
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655268397045-bcb9777f-8d71-4551-8df7-c383c9959a2c.png#averageHue=%23fec037&clientId=u9b9a6e72-ffc9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=335&id=u57e46ba1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=776&originWidth=1464&originalType=binary&ratio=1&rotation=0&showTitle=false&size=90838&status=done&style=shadow&taskId=ud86b2864-4276-44dd-9f1e-d54fa336e90&title=&width=632.857177734375)
<a name="CZaGY"></a>
#### 1.5
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655432068534-44e972a8-416f-4615-9a77-1466a647557b.png#averageHue=%23dcac43&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=492&id=u1c54de38&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1040&originWidth=1032&originalType=binary&ratio=1&rotation=0&showTitle=false&size=120115&status=done&style=shadow&taskId=uc440fd64-1f22-45c5-9319-4b492e43563&title=&width=488.28570556640625)
<a name="QjZAK"></a>
#### 1.6
所给程序片段不合法；<br />原因：<<输出运算符左侧必须是ostream对象，而第二、三行<<左侧均没有cout
<a name="iXHoc"></a>
#### 1.7
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655432815802-9e99017e-70e1-41cc-a760-c8a6afe96fa7.png#averageHue=%238fc162&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=397&id=ueeb58a16&margin=%5Bobject%20Object%5D&name=image.png&originHeight=732&originWidth=662&originalType=binary&ratio=1&rotation=0&showTitle=false&size=59310&status=done&style=shadow&taskId=u52a90ee5-8445-43e8-8e6e-a6c12f93277&title=&width=359.3809509277344)<br />报错显示如下：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655432888018-00846db8-f221-4fb4-8cfa-32bec61fec3b.png#averageHue=%23f7f6f5&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=147&id=uf597dff7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=193&originWidth=1412&originalType=binary&ratio=1&rotation=0&showTitle=false&size=56925&status=done&style=shadow&taskId=ud389aaa9-dfc5-44d8-a021-50608f892f0&title=&width=1075.8095238095239)
<a name="OUOAY"></a>
#### 1.8
第一、二行语句显然合法；<br />第三行<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655433262521-e6bfb9c6-02d2-4fd0-bd20-d5f14905909f.png#averageHue=%235ac868&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=357&id=uc29c410f&margin=%5Bobject%20Object%5D&name=image.png&originHeight=468&originWidth=684&originalType=binary&ratio=1&rotation=0&showTitle=false&size=43564&status=done&style=shadow&taskId=u33ca3984-c270-4d38-bd83-075fe20e075&title=&width=521.1428571428571)<br />可以看到编译器识别出一对/* */注释，而后面的内容当做字符串常量处理，少了一个"，则报错missing terminating " character<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655433275250-92ee2740-1e15-44f3-a540-d53a542bc1e1.png#averageHue=%23f8f8f7&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=222&id=u5a3112c5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=291&originWidth=782&originalType=binary&ratio=1&rotation=0&showTitle=false&size=37587&status=done&style=shadow&taskId=u08aa3e94-ad01-42d7-b1f4-aaf7f16595c&title=&width=595.8095238095239)<br />第四行代码会输出/*_，_而前后均为/* */注释
<a name="cnfWf"></a>
#### 1.9
sum of 50 to 100 inclusive意思是求和区间为[50,100]的闭区间<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655433967718-b3e83466-67dc-480f-b2e9-58dff38d3e60.png#averageHue=%23f4f4f4&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=130&id=uaff9caaa&margin=%5Bobject%20Object%5D&name=image.png&originHeight=170&originWidth=577&originalType=binary&ratio=1&rotation=0&showTitle=false&size=16673&status=done&style=shadow&taskId=u8938157f-d252-4cc2-8529-422cf0eb6c6&title=&width=439.6190476190476)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655434078701-0f2d4550-076d-4ef2-b528-8707a49ec0b6.png#averageHue=%23d2a645&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=364&id=u3d6e8ad4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=820&originWidth=1262&originalType=binary&ratio=1&rotation=0&showTitle=false&size=89191&status=done&style=shadow&taskId=u4f5e794f-da5d-4e4c-8369-9ff93970f73&title=&width=559.5238037109375)
<a name="sO4AA"></a>
#### 1.10
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655434539410-d565370c-7c00-4e13-9af7-37f2f63ec32a.png#averageHue=%23b0b665&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=427&id=u2fcc3a97&margin=%5Bobject%20Object%5D&name=image.png&originHeight=820&originWidth=804&originalType=binary&ratio=1&rotation=0&showTitle=false&size=72864&status=done&style=shadow&taskId=u70f00834-51f0-472a-a71c-acbb30786dd&title=&width=418.5714111328125)<br />没什么特殊情况最好还是--num
<a name="lEhbq"></a>
#### 1.11
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1655435041586-f833962d-60c0-4b05-ac35-fc005a5f5f9f.png#averageHue=%23fec037&clientId=u236ad75c-6ae9-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=373&id=u29dea1b0&margin=%5Bobject%20Object%5D&name=image.png&originHeight=952&originWidth=1280&originalType=binary&ratio=1&rotation=0&showTitle=false&size=103561&status=done&style=shadow&taskId=u19c23c2e-144a-4af0-bd5e-d8aa31c4478&title=&width=501.23809814453125)<br />当然上面程序健壮性不足，如果不按提示要求，输入a>b则达不到想要的结果（书上没看到if，姑且不优化了）
<a name="gecBz"></a>
## 1.4 控制流
<a name="FIogj"></a>
### while和for循环语句
循环中若不停检测变量并递增，使用for循环会更方便

---

读取数量不定的输入，如输入int至变量int value，可以写**while(cin>>value){...}**<br />使用istream对象作为条件，实际是检测对象状态，如果碰到无效输入或文件结束符end-of-file，循环会自动结束

- Unix MacOS为CTRL+D
- Windows为CTRL+Z
<a name="hescJ"></a>
#### 练习
<a name="Fpwsx"></a>
##### 1.12
此for循环完成了从-100到100的整数累加的功能，sum为和，结果自然为0
<a name="QGdz8"></a>
##### 1.13
即使用for循环重做1.9-1.11三道题<br />1.9重做：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1656078849597-ca6c4c05-a7a0-4b5b-a981-6c49bb8de282.png#averageHue=%23d2a748&clientId=ua72a1158-d410-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=497&id=u52281d12&margin=%5Bobject%20Object%5D&name=image.png&originHeight=820&originWidth=966&originalType=binary&ratio=1&rotation=0&showTitle=false&size=79685&status=done&style=shadow&taskId=uc3051acd-5482-4d13-b77f-912f0640764&title=&width=585.454511616186)<br />1.10重做：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1656079111445-e83d9bf0-b908-4723-889c-c3c88d358031.png#averageHue=%23b0b565&clientId=ua72a1158-d410-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=417&id=udd834207&margin=%5Bobject%20Object%5D&name=image.png&originHeight=688&originWidth=862&originalType=binary&ratio=1&rotation=0&showTitle=false&size=68531&status=done&style=shadow&taskId=u170d7ba8-027b-4017-ba69-f15a1990bdc&title=&width=522.4242122289362)<br />1.11重做：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1656079254152-0c41f756-bf6a-4564-957e-a5ba0bdeb5fc.png#averageHue=%23fec33f&clientId=ua72a1158-d410-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=524&id=u116e40b7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=864&originWidth=1052&originalType=binary&ratio=1&rotation=0&showTitle=false&size=81701&status=done&style=shadow&taskId=u685bce2d-1731-4ea8-b826-a8f117c7cf8&title=&width=637.5757207248733)
<a name="nVTqM"></a>
##### 1.14
区别主要是：

- while循环难以控制计数变量的作用域，循环体外依然有效；而for的控制变量一般只在循环内可见
- while更适合循环结束条件未知的场景（包括死循环和输入数量不定）；for一般用计数器迭代，循环次数已知

两者底层差别不大
<a name="JJ96a"></a>
##### 1.16
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1656080336849-92452193-5830-4565-8e53-ded35b10131c.png#averageHue=%23e4b244&clientId=ua72a1158-d410-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=497&id=ubf27358f&margin=%5Bobject%20Object%5D&name=image.png&originHeight=820&originWidth=946&originalType=binary&ratio=1&rotation=0&showTitle=false&size=73296&status=done&style=shadow&taskId=u9f36bb71-09b0-4205-86bd-6ddbf5d5a46&title=&width=573.333300195561)
<a name="o8eDE"></a>
### if语句
<a name="bVzPc"></a>
#### 练习
<a name="MV3VC"></a>
##### 1.17
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657881087523-f3a9684f-f566-4c45-b00f-795053766117.png#averageHue=%23f9f9f8&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=817&id=uc6d7cd4b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1348&originWidth=1758&originalType=binary&ratio=1&rotation=0&showTitle=false&size=173456&status=done&style=shadow&taskId=uc8b4ab8c-e836-49b0-8de8-70d95e25967&title=&width=1065.4544838729348)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657881096245-6f032f9d-9cfc-4bd8-beda-f71901188ee7.png#averageHue=%23f1efee&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=179&id=ufe60caea&margin=%5Bobject%20Object%5D&name=image.png&originHeight=296&originWidth=320&originalType=binary&ratio=1&rotation=0&showTitle=false&size=19803&status=done&style=shadow&taskId=u50179774-371b-4977-975c-53f30dec33c&title=&width=193.9393827299995)
<a name="qvDAJ"></a>
##### 1.19
对练习1.11进行优化<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657881362362-63ca6971-1468-40e7-a226-1ccfcf0157fb.png#averageHue=%23fec23d&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=759&id=u5e3574c6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1252&originWidth=1126&originalType=binary&ratio=1&rotation=0&showTitle=false&size=126766&status=done&style=shadow&taskId=uf55f0ea9-b5d3-472a-af1e-06eb2bcd8db&title=&width=682.4242029811858)
<a name="U9ujX"></a>
## 1.5 类简介
<a name="UClZQ"></a>
### Sales_item类
例程为定义一个Sales_item的类，表示书的总销售额、售出册数和平均售价；<br />操作为<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657881568933-e32c0e9c-0026-4662-ae76-d793ba07e7f7.png#averageHue=%23ededed&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=238&id=uc188ad7d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=393&originWidth=1295&originalType=binary&ratio=1&rotation=0&showTitle=false&size=332105&status=done&style=shadow&taskId=ude6eb4cd-54e8-4001-a06c-fd5b235423f&title=&width=784.8484394854668)
<a name="stEf2"></a>
#### 练习
<a name="p9eB7"></a>
##### 1.21
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657882448032-c0a94433-87a4-4178-84e4-68cbb0f839d7.png#averageHue=%23ddac41&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=468&id=u33039e7e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=772&originWidth=990&originalType=binary&ratio=1&rotation=0&showTitle=false&size=81969&status=done&style=shadow&taskId=u11feab23-28f0-495f-aa64-eb78a7ac871&title=&width=599.999965320936)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657882442362-26856bc9-2b86-489c-a523-e7295b5e25e8.png#averageHue=%23efeeec&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=72&id=Csb3Y&margin=%5Bobject%20Object%5D&name=image.png&originHeight=119&originWidth=634&originalType=binary&ratio=1&rotation=0&showTitle=false&size=13098&status=done&style=shadow&taskId=u59d305db-d991-4185-ba58-b2945d0db8b&title=&width=384.2424020338115)
<a name="PCHeC"></a>
##### 1.22
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657882583233-8e594443-458f-4d13-bb7a-bb52bb052fae.png#averageHue=%23ddac3f&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=584&id=uf75cac65&margin=%5Bobject%20Object%5D&name=image.png&originHeight=964&originWidth=970&originalType=binary&ratio=1&rotation=0&showTitle=false&size=94586&status=done&style=shadow&taskId=u26de075c-1e6c-4f08-affb-b2397ec7e44&title=&width=587.878753900311)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657882573705-05b85cb2-6366-42b1-80d9-d8f26925775b.png#averageHue=%23f2f1f0&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=108&id=u79f81292&margin=%5Bobject%20Object%5D&name=image.png&originHeight=178&originWidth=706&originalType=binary&ratio=1&rotation=0&showTitle=false&size=16221&status=done&style=shadow&taskId=udb655c45-effe-4477-9427-9812770fd62&title=&width=427.8787631480614)
<a name="KCMMI"></a>
##### 1.23&1.24
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657883045959-88400b11-a415-4082-89dd-6a8ba5afa48a.png#averageHue=%23f9f9f8&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=817&id=ue6dc78a7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1348&originWidth=1838&originalType=binary&ratio=1&rotation=0&showTitle=false&size=168620&status=done&style=shadow&taskId=uf3c68dba-8eaf-4b22-9ce8-98875fa7c22&title=&width=1113.9393295554346)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657883055461-94fecc50-90d8-47e0-b7fd-fc06732010ba.png#averageHue=%23f5f4f3&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=143&id=u1302859d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=236&originWidth=307&originalType=binary&ratio=1&rotation=0&showTitle=false&size=9416&status=done&style=shadow&taskId=ua09aa1c3-efbd-49fa-a29e-2c80b35323b&title=&width=186.06059530659326)
<a name="xBIlf"></a>
## 1.6 书店程序
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657897051522-35933428-abb9-4e2d-a5a0-cf598990ae99.png#averageHue=%23fbfafa&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=449&id=ua36ba767&margin=%5Bobject%20Object%5D&name=image.png&originHeight=3300&originWidth=2742&originalType=binary&ratio=1&rotation=0&showTitle=false&size=279243&status=done&style=shadow&taskId=u61e5fafa-6ade-4559-87ad-e7e32441cf1&title=&width=372.9526062011719)

<a name="SF3Tr"></a>
# 第2章 变量和基本类型——第Ⅰ部分 C++基础
C++由于和硬件高度相关，没有规定数据类型必须使用多少位存储，使用时需要依据机器和编译器灵活判断；
<a name="ht5YO"></a>
## 2.1 基本内置类型
<a name="BYRNZ"></a>
### 算术类型
一些建议：

- 数确定不为负，使用无符号类型
- 整型要么char，要么int，更大用long long
- 浮点型都用double
- bool=true or false

部分整数类型的内存大小，我的机器应该是LLP64的标准<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658159981455-e67bc621-cebf-46d4-8d26-163ab124ad53.png#averageHue=%23f3f2f2&clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=602&id=ub3c71b2c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=994&originWidth=1156&originalType=binary&ratio=1&rotation=0&showTitle=false&size=112105&status=done&style=shadow&taskId=uaa485ca2-f687-40e2-92b1-1442a0bc856&title=&width=700.6060201121232)
<a name="ZTSvh"></a>
### 类型转换
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657897902577-15cbfc9d-b7de-4514-b4ef-501bfbd13d2a.png#averageHue=%23efefef&clientId=u63c8daf2-4bc7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=521&id=u6be036d4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=859&originWidth=1388&originalType=binary&ratio=1&rotation=0&showTitle=false&size=676835&status=done&style=shadow&taskId=ud62254c0-3e55-4a8d-b76f-75a798e535c&title=&width=841.2120725913728)<br />**含有无符号类型的表达式**<br />带符号数会自动转换成无符号数，负数转unsigned会加上无符号数的模<br />//在32位系统中，int的范围是-2147483648~+2147483647，而unsigned int的范围是0~4294967295<br />例：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657941823380-4df57092-c3f9-40ab-9dfd-0f329b6af58c.png#averageHue=%23f9f8f7&clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=295&id=u641bcb39&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1458&originWidth=1644&originalType=binary&ratio=1&rotation=0&showTitle=false&size=92875&status=done&style=shadow&taskId=ud7577828-9cd4-472e-8a00-af609221db8&title=&width=332.36358642578125)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657941859040-22ff60f6-d000-413a-9df2-3bddaf98994c.png#averageHue=%23f8f7f7&clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=215&id=u467c574f&margin=%5Bobject%20Object%5D&name=image.png&originHeight=355&originWidth=1160&originalType=binary&ratio=1&rotation=0&showTitle=false&size=26282&status=done&style=shadow&taskId=u673996b2-18f1-4a8c-a2ea-171eff6c548&title=&width=703.0302623962482)
<a name="ndjEz"></a>
#### 练习
<a name="qSETh"></a>
##### 2.3
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657942574531-b0d9b91d-aacd-48e7-95b5-6edd700db99e.png#averageHue=%23262c32&clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=295&id=u579ad4c7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=1680&originalType=binary&ratio=1&rotation=0&showTitle=false&size=119202&status=done&style=shadow&taskId=u332d2258-79b1-4f91-b826-64e3d57d8e1&title=&width=287.1817626953125)<br />从上到下分别应输出<br />32 <br />4294967264= 4294967296 - 32<br />32<br />-32<br />0<br />0
<a name="nRckZ"></a>
### 字面值常量literal
整型默认int，浮点型默认double，字符型为char；<br />字符串为C风格数组，实质是const char*

---

转义字符<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657944100033-7b60e812-0761-4758-941b-61457a734fcb.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=113&id=u7882b022&margin=%5Bobject%20Object%5D&name=image.png&originHeight=186&originWidth=1143&originalType=binary&ratio=1&rotation=0&showTitle=false&size=91041&status=done&style=shadow&taskId=u205159a3-8dea-4cc6-9b77-2d8000ae1f3&title=&width=692.727232688717)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657944158972-691e7398-4fc0-47b7-ac53-b8fd08c66f00.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=383&id=ub00d908a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=632&originWidth=1336&originalType=binary&ratio=1&rotation=0&showTitle=false&size=316520&status=done&style=shadow&taskId=u4807cf3f-cb6a-43b3-b4e1-a430458b1a6&title=&width=809.6969228977479)
<a name="ImZz1"></a>
## 2.2 变量
<a name="ntSoZ"></a>
### 列表初始化
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657944411905-eae92188-2ab0-4eba-877e-bd5fa7e3812a.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=118&id=u24ed00e6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=194&originWidth=485&originalType=binary&ratio=1&rotation=0&showTitle=false&size=40527&status=done&style=shadow&taskId=u6018fe9a-f5f2-44ec-a635-b0d0560658b&title=&width=293.9393769501555)<br />四种初始化方式中，只有列表初始化在丢失信息时会报错，如long double值给int初始化
<a name="Wqgei"></a>
### 默认初始化
内置类型函数外为0，**函数内为垃圾值**；<br />对象默认值由类决定
<a name="c1hJA"></a>
#### 练习
<a name="EdggZ"></a>
##### 2.9
（a）应该为int input_value;	cin>>input_value<br />（b）不符合初始化语法，见列表初始化<br />（c）wage未定义	![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657945227175-e199e989-1807-4d95-a5f5-b4bc8843bc01.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=53&id=u04518069&margin=%5Bobject%20Object%5D&name=image.png&originHeight=87&originWidth=625&originalType=binary&ratio=1&rotation=0&showTitle=false&size=8941&status=done&style=shadow&taskId=u3c668516-988a-4872-a77a-a73d8fda12a&title=&width=378.78785689453025)<br />（d）语法没问题，只是i将初始化为3，小数点后截断
<a name="v4EA8"></a>
##### 2.10
global_str为空串<br />global_int为0<br />local_int为随机值<br />local_str为空串
<a name="n98CI"></a>
### 变量声明与定义
加extern为声明，其他全为定义，会分配存储空间和初始化<br />//extern初始化同样是定义
<a name="MZOot"></a>
#### 练习
<a name="RWi54"></a>
##### 2.11
（a）定义<br />（b）定义<br />（c）声明
<a name="EZTt7"></a>
### 标识符
字母、数字、下划线组成，字母、下划线开头；

- 自定义不允许连续两个下划线
- 不允许下划线+大写字母开头
- 全局变量不能以下划线开头

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657946197388-1819d06e-d0df-47d4-b5b9-2313d748db0f.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=612&id=u0ba53594&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1009&originWidth=1348&originalType=binary&ratio=1&rotation=0&showTitle=false&size=569880&status=done&style=shadow&taskId=u0db21287-9c9c-41a4-bc3c-7bea8269525&title=&width=816.9696497501229)
<a name="hiZls"></a>
#### 练习
<a name="zJroY"></a>
##### 2.12
(a)(c)(d)非法，不能含连字符，不能数字开头，不能用关键字
<a name="ErnUu"></a>
### 名字作用域
<a name="CKMEX"></a>
#### 练习
<a name="VLkYP"></a>
##### 2.13
j=100
<a name="IgklJ"></a>
##### 2.14
输出100 55
<a name="dxXaA"></a>
## 2.3 复合类型
<a name="PUu9r"></a>
### 引用
引用/**左值引用**即别名，和**对象**绑定而不是拷贝；**必须初始化**<br />一般来说，引用的类型和绑定的对象应一致
<a name="vFNE1"></a>
#### 练习
<a name="LLhy2"></a>
##### 2.15
(b)(d)不合法，引用不可以绑定字面值，引用必须初始化
<a name="yzA4n"></a>
##### 2.16
都合法，只是有些副作用<br />(b)会执行int到double的隐式转换<br />(c)(d)小数点后会截断
<a name="E1OrI"></a>
##### 2.17
输出10 10
<a name="E1zk1"></a>
### 指针
类似于内置类型，指针存地址，解析取决于指向类型；<br />一般情况也要类型匹配

---

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657947389399-8c388364-ed88-40b0-ae1b-b1b41f726f77.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=199&id=ue47c0a5d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=328&originWidth=794&originalType=binary&ratio=1&rotation=0&showTitle=false&size=127494&status=done&style=shadow&taskId=uec8e7dba-9f83-4dbc-80d1-527120c6544&title=&width=481.21209339881125)<br />无效指针（包括未初始化的）不要使用，可能指向危险地址；空指针初始化为nullptr，NULL和0相同，不过新标准还是用nullptr；

---

void*指针无法访问其指向对象，操作有限；<br />指针比较的是存的地址；只要不为空指针，指针的值就不是0
<a name="ZrU6v"></a>
#### 练习
<a name="YCpFc"></a>
##### 2.20
定义指针p1指向i；<br />通过指针使i平方一次
<a name="zntG3"></a>
##### 2.21
(a)非法，类型不匹配；(b)非法，int不可以初始化int*，即使int=0；(c)合法
<a name="kQu8W"></a>
##### 2.25
(a)ip是int型指针，i是int型变量，r是i的引用<br />(b)i是int型变量，ip是int型空指针<br />(c)ip是int型指针，ip2是int型变量
<a name="bjGoy"></a>
## 2.4 const限定符
const默认作用域为当前文件；<br />共享需要在声明和定义时都加extern
<a name="B0Qpx"></a>
#### 练习
<a name="xViqu"></a>
##### 2.26
(a)(d)非法，const常量必须初始化，不可被改变；(b)(c)合法
<a name="JDyQw"></a>
### const引用
初始化常量引用时允许用任意表达式作初始值，只要能转换为引用类型即可<br />const引用本质是不允许通过引用改变引用对象的值，而引用对象是不是const无关紧要<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657955352236-1b4c223f-200a-4b30-aa6f-183bda3245b6.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=142&id=uf69938d7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=234&originWidth=739&originalType=binary&ratio=1&rotation=0&showTitle=false&size=17056&status=done&style=shadow&taskId=ueaec0abd-8e6f-46a4-9a1e-41ca4234f6d&title=&width=447.8787619920926)比如此处不可以通过ri改变dval的值<br />但是**常量只可以用const引用**，因为非const引用可能改变常量的值，C++将此视为非法<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657955499121-21862554-b242-4743-8862-059132fba6c9.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=101&id=u8b572496&margin=%5Bobject%20Object%5D&name=image.png&originHeight=166&originWidth=936&originalType=binary&ratio=1&rotation=0&showTitle=false&size=18407&status=done&style=shadow&taskId=ue898bedf-9ca8-4aa5-81dd-a1e2bff44c4&title=&width=567.2726944852485)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657955516409-790f1fd6-9001-4aa6-a7b9-2e281eafba4c.png#clientId=ue8e4867b-bbd7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=96&id=u6fcc917c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=158&originWidth=1960&originalType=binary&ratio=1&rotation=0&showTitle=false&size=33124&status=done&style=shadow&taskId=uf254d90b-d2c6-4a57-8052-f59f7bd4c37&title=&width=1187.878719221247)
<a name="eOZa0"></a>
### 指针和const
const指针与const引用类似<br />（指针或引用自以为是，它们觉得自己指向了常量）

---

指针常量指the pointer itself is const<br />语法是把*放在const之前，表明指针将不会改变指向<br />但是能否通过指针改变对象值完全取决于对象是否是const，和指针常量无关
<a name="eJlUg"></a>
#### 练习
<a name="t64xT"></a>
##### 2.27
(a) 不合法，引用不能引用字面值<br />(f) 不合法，引用本身就和对象绑定，引用默认就是引用常量，& const不是合法声明<br />其他语句均合法
<a name="M6kJD"></a>
##### 2.28
(a)(b)(d)均不合法，指针常量和const常量没有区别，必须初始化<br />(c)不合法是因为ic是const常量没有初始化<br />(e)合法，const指针不是常量不需要初始化
<a name="Syb3K"></a>
##### 2.29
(b)不合法，不可以绕道通过p1修改p3指向的对象，**禁止非const指针赋值给const指针**<br />(c)不合法，非const指针不可以指向const常量，否则可以通过指针修改const常量，而这不符合设计要求<br />其他语句合法
<a name="IeX4b"></a>
### 顶/底层const
顶层const表示指针、算术类型、类本身是常量；<br />底层const表示指针、引用指向的对象是常量<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657973429643-457a3b1f-6084-4735-95d4-6dbb1c73540c.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=114&id=u065e350b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=188&originWidth=1108&originalType=binary&ratio=1&rotation=0&showTitle=false&size=98534&status=done&style=shadow&taskId=u947b03d5-b694-4238-9c03-382dd928290&title=&width=671.5151127026232)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657973437096-f09a332c-3b13-49be-8338-b9413f2f33f1.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=65&id=u927f13dc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=107&originWidth=1249&originalType=binary&ratio=1&rotation=0&showTitle=false&size=71208&status=done&style=shadow&taskId=u94823fb2-9037-4bcb-b567-cf12ae61834&title=&width=756.9696532180293)<br />指针可以是顶层const也可以是底层const；<br />赋值操作时，两者需要具有相同的底层const（=忽略顶层const），或数据类型可以相互转换；一般来说就是非const可以赋值const，反之则非法。
<a name="NuzXl"></a>
#### 练习
<a name="tgwY0"></a>
##### 2.30
v2 是顶层const，p2 是底层const，p3 既是顶层const又是底层const，r2 是底层const。
<a name="L8nYz"></a>
##### 2.31
√×√×√
<a name="oq5qp"></a>
### constexpr和常量表达式
**编译过程**中可得到**定值**才是常量表达式；

- 用常量表达式初始化的const变量、字面值也是常量表达式
- 函数返回值和非const对象都不是常量表达式（constexpr函数除外）
<a name="WX01u"></a>
#### constexpr
如果认定变量或函数是常量表达式，就声明为constexpr型；有点像const的加强版<br />算术类型、引用、指针可定义为constexpr

- constexpr指针初始化值必须是常量
- 如nullptr、0、地址不变的对象
- 函数内部变量地址一般都会变，不可以初始化constexpr指针，而全局变量可以
- constexpr指针是指针常量
<a name="JWDuq"></a>
#### 练习
<a name="AzajO"></a>
##### 2.32
不可以用int值初始化int指针，要么强制转换int为int*，要么用字面值0或nullptr或NULL
<a name="CT1t8"></a>
## 2.5 处理类型
<a name="AfVzN"></a>
### 类型别名

- typedef/#define<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657975730856-dcdad6cb-c7c9-4c50-9d88-f187020893fe.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=59&id=QKmrF&margin=%5Bobject%20Object%5D&name=image.png&originHeight=97&originWidth=1276&originalType=binary&ratio=1&rotation=0&showTitle=false&size=70310&status=done&style=shadow&taskId=ucae35c89-e2f5-4087-b6a3-d7fe1722fb2&title=&width=773.333288635873)<br />但是typedef数组的别名真的难理解/反人类。。
- using newname = oldname<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657975791089-09cc3898-83ab-4e50-9455-24c35f2c5032.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=39&id=u576c0f6b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=64&originWidth=1025&originalType=binary&ratio=1&rotation=0&showTitle=false&size=27678&status=done&style=shadow&taskId=u0f142edf-4e8d-444d-b284-4c07c08ddad&title=&width=621.2120853070296)

指针、引用等的别名见到const之后要注意理解<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657975941361-d072263a-12d1-48fc-8826-3325ff0da596.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=77&id=u9be5d7bd&margin=%5Bobject%20Object%5D&name=image.png&originHeight=127&originWidth=1262&originalType=binary&ratio=1&rotation=0&showTitle=false&size=86514&status=done&style=shadow&taskId=u032cc5fd-42ce-4601-903a-0768e78567e&title=&width=764.8484406414356)<br />不能理解为![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657975988553-5b62d1c5-8edf-4465-bc40-3782ec3a8a9a.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=38&id=u472e7c02&margin=%5Bobject%20Object%5D&name=image.png&originHeight=62&originWidth=491&originalType=binary&ratio=1&rotation=0&showTitle=false&size=11613&status=done&style=shadow&taskId=u74074e73-b5ca-4663-b161-ae213a9758a&title=&width=297.575740376343)<br />**const是对给定类型的修饰，pstring是指向char的指针，那么const pstring就是指向char的指针常量，也就是pstring不变/指针不变**<br />不可以像宏一样简单替换
<a name="fZ1Ax"></a>
### auto类型说明符

- auto一般忽略顶层const，保留底层const
- 需要顶层const时需要写const auto或者使用**auto引用<br />**auto引用会给出引用对象的类型，此时不会忽略顶层const了
- 一行声明中变量类型应相同<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658112312530-79c562c2-7251-437f-adb5-664debfec0e1.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=36&id=u2892f783&margin=%5Bobject%20Object%5D&name=image.png&originHeight=60&originWidth=909&originalType=binary&ratio=1&rotation=0&showTitle=false&size=25857&status=done&style=shadow&taskId=u10a3db72-e66a-4248-a37d-2abb6093760&title=&width=550.9090590674049)

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657976571823-63ff1b65-7e54-42d4-b4ff-45999929ea56.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=113&id=u6a921cdd&margin=%5Bobject%20Object%5D&name=image.png&originHeight=432&originWidth=1368&originalType=binary&ratio=1&rotation=0&showTitle=false&size=45284&status=done&style=shadow&taskId=u4c46f916-b24d-491f-bede-b97689e5fa3&title=&width=357.0889892578125)
<a name="MtvnI"></a>
#### 练习
<a name="tORw4"></a>
##### 2.35
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1657976814945-b5dd26e0-db43-48bf-bfa9-e03ca33ec4d4.png#clientId=u9f708f24-bee8-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=163&id=uc04d8b42&margin=%5Bobject%20Object%5D&name=image.png&originHeight=720&originWidth=2682&originalType=binary&ratio=1&rotation=0&showTitle=false&size=101849&status=done&style=shadow&taskId=u493dae2c-ecf0-415c-ad90-f38b8b345be&title=&width=606.9469604492188)
<a name="nqmEC"></a>
### decltype
decltype不会真的执行（）中的表达式或函数，只是推断

- decltype(variable)<br />当变量是引用时返回引用，否则变量是什么就返回什么（包括顶层const和引用）
- decltype((variable))<br />把(variable)当表达式，为特殊左值，返回引用
- decltype(expression)<br />当表达式是左值时，返回引用，如指针解引用，否则返回表达式结果类型
<a name="nxYIZ"></a>
#### 练习
<a name="h6EJI"></a>
##### 2.36
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658028206275-541a9659-9247-4519-a46a-3bdafe1f90a2.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=206&id=u5ef93052&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1008&originWidth=2550&originalType=binary&ratio=1&rotation=0&showTitle=false&size=98375&status=done&style=shadow&taskId=u799aef9b-b2e1-41a1-afeb-73146f769c4&title=&width=520.973388671875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658028220314-2d66a379-d651-4834-8631-a5e2589d73ae.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=203&id=u7d30b285&margin=%5Bobject%20Object%5D&name=image.png&originHeight=407&originWidth=1168&originalType=binary&ratio=1&rotation=0&showTitle=false&size=33259&status=done&style=shadow&taskId=u33c79ec3-d93e-4748-a02b-ba558e68c35&title=&width=581.8787231445312)
<a name="MpIij"></a>
##### 2.37
！赋值操作符会返回左值引用<br />一种解释是对象在赋值的时候，返回引用比返回临时对象开销要更小，效率更高<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658028664836-e9ee6fcd-ad7c-422b-a10a-cd67f1849d91.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=110&id=u7e83ec44&margin=%5Bobject%20Object%5D&name=image.png&originHeight=182&originWidth=1121&originalType=binary&ratio=1&rotation=0&showTitle=false&size=17060&status=done&style=shadow&taskId=ua4c17932-a5c9-4040-a1f3-0a06ae3ffe8&title=&width=679.3939001260295)<br />所以本题中int a=3; int b=4; int c=3; int &d=a=3
<a name="Rol8X"></a>
##### 2.38
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658028961029-682e9864-ea02-4019-9a46-a84d164c76ae.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=147&id=ua5c317a4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=243&originWidth=1190&originalType=binary&ratio=1&rotation=0&showTitle=false&size=35293&status=done&style=shadow&taskId=u6eb5e380-e48f-4951-9c34-67082712067&title=&width=721.2120795271857)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658029009475-0f9f7010-e80a-4a58-87bd-bcee475de17b.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=160&id=ua19ad3a4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=432&originWidth=1290&originalType=binary&ratio=1&rotation=0&showTitle=true&size=37075&status=done&style=shadow&taskId=ua2cc09f5-a94a-4268-9728-d53cf5b9c61&title=decltype%E5%92%8Cauto%E4%BD%9C%E7%94%A8%E7%9B%B8%E5%90%8C&width=477.818115234375 "decltype和auto作用相同")![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658029044629-19841b6c-8289-44f4-a6dd-be7081728b3a.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=158&id=u5d24e733&margin=%5Bobject%20Object%5D&name=image.png&originHeight=432&originWidth=1548&originalType=binary&ratio=1&rotation=0&showTitle=true&size=46884&status=done&style=shadow&taskId=u5b262db6-acd1-42bd-b64e-f88d771c04c&title=decltype%E5%92%8Cauto%E4%BD%9C%E7%94%A8%E4%B8%8D%E5%90%8C&width=566.1760864257812 "decltype和auto作用不同")
<a name="UPNFt"></a>
## 2.6 自定义数据结构
C++中的 struct 和 class 基本是通用的，唯有几个细节不同：

- 使用 class 时，类中的成员默认都是 private 属性的；而使用 struct 时，结构体中的成员默认都是 public 属性的。
- class 继承默认是 private 继承，而 struct 继承默认是 public 继承
- class 可以使用模板，而 struct 不能
<a name="fEP4v"></a>
#### 练习
<a name="LACSq"></a>
##### 2.39
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658029742778-5ca80553-fdc4-41e0-858b-c52ec6762ae1.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=94&id=u91b87111&margin=%5Bobject%20Object%5D&name=image.png&originHeight=155&originWidth=1423&originalType=binary&ratio=1&rotation=0&showTitle=false&size=17181&status=done&style=shadow&taskId=u62a9c06b-35cd-433e-a8c1-0a6082bced5&title=&width=862.4241925774666)<br />提醒类或结构体定义后加分号

---

头文件保护符习惯性加上即可<br />#ifndef<br />#define<br />...<br />#endif
<a name="FFVKu"></a>
# 第3章 字符串、向量和数组
//<iostream>间接包含了<string>，但是有保护符，不会重复包含；编译时可以-M查看包含的头文件
<a name="nxzcF"></a>
## 3.2 标准库类型string
其实是basic_string<char>模板类
<a name="wGGW0"></a>
### 定义和初始化string对象
标准定义了很多初始化方式，十几种，常用的如下：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658030714768-76a982d9-9190-494d-af96-eba8a061a50f.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=241&id=udbf5f096&margin=%5Bobject%20Object%5D&name=image.png&originHeight=397&originWidth=1335&originalType=binary&ratio=1&rotation=0&showTitle=false&size=283085&status=done&style=shadow&taskId=u8b0545cf-866c-4f39-ae16-97ac34c9204&title=&width=809.0908623267167)

---

上述初始化方法第4和第5应该还是保留了字符串字面值尾部的'\0'（虽然书上说没有）；<br />size函数返回size_type类型，由于是无符号数，尽量不用int；
<a name="hKlSe"></a>
#### 练习
<a name="tX6kx"></a>
##### 3.2
修改前![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658064574221-c66adc1c-cf7d-4f8d-a346-e38cca3472eb.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=65&id=uec5e70f0&margin=%5Bobject%20Object%5D&name=image.png&originHeight=432&originWidth=3018&originalType=binary&ratio=1&rotation=0&showTitle=false&size=54344&status=done&style=shadow&taskId=u90e9ec6d-f770-4895-9ede-db051cf4c37&title=&width=450.973388671875)<br />修改后![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658064650115-2f9dc068-3dfa-460c-969b-dd2a9ce37a22.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=67&id=u042b215a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=432&originWidth=2898&originalType=binary&ratio=1&rotation=0&showTitle=false&size=51469&status=done&style=shadow&taskId=u2b3dca20-b117-498d-8aec-bb1397c6f5d&title=&width=449.960205078125)
<a name="OHu1l"></a>
##### 3.3
string输入运算符碰到空白字符会截断，包括制表符、空格和换行符；<br />getline只会截止在换行符
<a name="DNvxB"></a>
##### 3.4
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658065310783-9c8ecf18-9f41-4378-b5f2-dc7f3659a4b4.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=432&id=u794d9d38&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=3996&originalType=binary&ratio=1&rotation=0&showTitle=true&size=172306&status=done&style=shadow&taskId=ude1d75a9-ac0b-41a7-887b-5b77e123926&title=%E6%AF%94%E8%BE%83%E5%AD%97%E7%AC%A6%E4%B8%B2&width=999 "比较字符串")![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658065445741-863f24bc-ad50-4684-90f1-bf645fc9426b.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=432&id=ua361d8ea&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=4926&originalType=binary&ratio=1&rotation=0&showTitle=true&size=189216&status=done&style=shadow&taskId=u3783ed47-b243-4ea7-8cde-d978518aa9f&title=%E5%AD%97%E7%AC%A6%E4%B8%B2%E9%95%BF%E5%BA%A6&width=1232 "字符串长度")

---

<a name="jD8VJ"></a>
### 处理string对象中的字符
**<cctype>**中有字符操作和判断库函数<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658065737561-5b82d0d0-c419-466b-83d7-8cb2b18f7e97.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=490&id=u2bca56ce&margin=%5Bobject%20Object%5D&name=image.png&originHeight=809&originWidth=1340&originalType=binary&ratio=1&rotation=0&showTitle=false&size=508543&status=done&style=shadow&taskId=u86ef8de9-b054-4d9d-a331-53772ed974b&title=&width=812.1211651818729)<br />去掉.h前面加c的头文件是C++从C继承来加上namespace的头文件；<br />范围for语句可以遍历容器中每一个元素，但是只访问一部分元素时不太好用了
<a name="X3cZ0"></a>
#### 练习
<a name="FsK3U"></a>
##### 3.6
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658066339267-2c29ea80-56f1-441a-bc75-d4bd1e3a2e1f.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=432&id=u6dd947de&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=1272&originalType=binary&ratio=1&rotation=0&showTitle=false&size=107869&status=done&style=shadow&taskId=ue2929fae-fa4c-451b-babd-5f9141a89b0&title=&width=318)
<a name="Go3Hv"></a>
##### 3.7
结果没变，也就是说string元素还是char类型
<a name="hhDzU"></a>
##### 3.8
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658066486069-edbba8a2-502d-4a71-af0f-0f9952f7a1c2.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=432&id=u89423247&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=2376&originalType=binary&ratio=1&rotation=0&showTitle=false&size=124752&status=done&style=shadow&taskId=ua355ede7-8536-4bb0-8508-c9fe44f3c6b&title=&width=594)<br />如果遍历所有元素还是范围for更好用了，但是也不一定
<a name="z25kH"></a>
##### 3.9
合法，输出s第一个元素；但没有意义，不显式初始化的string里面存的可能是垃圾值<br />[https://github.com/huangmingchuan/Cpp_Primer_Answers/tree/master/ch03](https://github.com/huangmingchuan/Cpp_Primer_Answers/tree/master/ch03)但是这个人说不合法，书上说C++标准不要求检测下标，而且实际使用中是可以这么写的虽然很危险
<a name="F1KWL"></a>
##### 3.10
用空白字符串接收处理原字符串的结果<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658068061649-45ab7db7-a4bf-4a83-a043-86e74cff26b0.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=468&id=ua50defcc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1872&originWidth=1560&originalType=binary&ratio=1&rotation=0&showTitle=false&size=135687&status=done&style=shadow&taskId=u60c35aff-c004-47ab-9219-23fe087d210&title=&width=390)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658068075926-a3da941d-b150-40ac-a831-6f711114fa57.png#clientId=u34be66d1-fad5-4&crop=0&crop=0.058&crop=1&crop=1&from=paste&height=190&id=u9c06adcc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=313&originWidth=1179&originalType=binary&ratio=1&rotation=0&showTitle=false&size=33332&status=done&style=shadow&taskId=u12308386-5fc7-42a1-8b44-dff3f68e783&title=&width=715)
<a name="wDEp5"></a>
##### 3.11
除循环内代码合法，c是const char&，因为不会允许通过c改变const string中的元素
<a name="CqOWY"></a>
## 3.3 标准库类型vector
vector包含对象类型都相同，是一个类模板；<br />尖括号中类型帮助编译器进行实例化（instantiation），且必须指定类型（引用除外）
<a name="gfNHO"></a>
### 定义和初始化vector对象
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658068453670-c2eb0a77-c602-4605-95d8-843a5792ff61.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=275&id=u78525c0c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=454&originWidth=1332&originalType=binary&ratio=1&rotation=0&showTitle=false&size=360058&status=done&style=shadow&taskId=u7528573a-50d0-47f6-9cc1-efe051c61d9&title=&width=807.2726806136229)<br />方法4、5是值初始化，6、7是列表初始化；<br />如果元素类型不支持默认初始化，那不能用5这种方法；<br />列表初始化会**尽量**被当成元素值的列表，如果无法这么做，会用给的值构造重复元素然后默认初始化<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658068920141-6ee97961-7a2a-41e2-bbf7-65bf71c1510c.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=107&id=u173a6a25&margin=%5Bobject%20Object%5D&name=image.png&originHeight=177&originWidth=1307&originalType=binary&ratio=1&rotation=0&showTitle=false&size=134614&status=done&style=shadow&taskId=u570fce24-1b63-4b37-af79-cbd1ae1688c&title=&width=792.1211663378417)<br />只有v5是列表初始化，v7，v8都和（）初始化等价，被当作构造vector对象的参数而不是元素值
<a name="LP1pA"></a>
#### 练习
<a name="uWEtu"></a>
###### 3.12
(a)(c)合法，(b)类型不同的vector不可以拷贝初始化
<a name="FB5YL"></a>
##### 3.13
(a)无元素；<br />(b)10个0<br />(c)10个42<br />(d)1个10<br />(e)10和42<br />(f)10个默认string（空串）<br />(g)10个hi
<a name="WIxCr"></a>
### 向vector对象中添加元素
事先指定vector大小可能导致性能更差，应该运行时动态添加元素；<br />范围for不要改变容器大小
<a name="q0OLD"></a>
#### 练习
<a name="n0QTF"></a>
##### 3.14
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658070394697-58ad0ce9-b0bd-4bf4-9406-dc9f112de853.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=541&id=u87986022&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2160&originWidth=1446&originalType=binary&ratio=1&rotation=0&showTitle=false&size=157360&status=done&style=shadow&taskId=ud63ec57d-7a2f-49df-b64b-ec2defe6428&title=&width=362)<br />3.15略，改变类型即可

---

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658070506588-5da86071-9ff4-434e-9602-8469cd3a1875.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=56&id=u02b55b92&margin=%5Bobject%20Object%5D&name=image.png&originHeight=93&originWidth=689&originalType=binary&ratio=1&rotation=0&showTitle=false&size=94030&status=done&style=shadow&taskId=ueaf1854c-88ac-4182-9768-ef3154c5143&title=&width=417.5757334405302)<br />由于vector是模板，尖括号指定类型才和类起相同作用，所以第二种写法不合法；<br />元素类型可以比较时才可以使用<、>等比较运算符；<br />下标只可以访问已有元素，如果访问不存在的元素将导致错误，但是编译器发现不了，如：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658070831731-8fe9685f-017a-492a-b404-0fb4416bb8af.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=324&id=udce26947&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1296&originWidth=1446&originalType=binary&ratio=1&rotation=0&showTitle=false&size=104099&status=done&style=shadow&taskId=u3aeca30f-91bd-430e-9649-2e5cca3ec1c&title=&width=362)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658070845007-f4e7340a-017c-4f49-992d-365c99639c46.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=249&id=uf1b6eec4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=411&originWidth=1179&originalType=binary&ratio=1&rotation=0&showTitle=false&size=34410&status=done&style=shadow&taskId=u11b891e7-a14d-4c7d-8cf1-f6eec0b9d9e&title=&width=714.5454132458419)<br />程序返回代码为异常
<a name="ggmr7"></a>
#### 练习
<a name="ETuOP"></a>
##### 3.17
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658076789767-e1ea9cde-b82f-4ee9-9572-2e74b6d83e52.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=450&id=uad911d74&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2736&originWidth=2256&originalType=binary&ratio=1&rotation=0&showTitle=false&size=268901&status=done&style=shadow&taskId=u54cfb2a1-185c-4ff8-9c12-dfe00b46276&title=&width=370.9867248535156)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658076888063-585f298f-97b1-480b-8be0-af80b6bb8099.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=317&id=ud1983e0c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=523&originWidth=1189&originalType=binary&ratio=1&rotation=0&showTitle=false&size=50022&status=done&style=shadow&taskId=uc5124921-1eef-4927-8f23-1e7b5a78105&title=&width=720.6060189561543)<br />第一行乱码可能是编码问题，按链接[https://www.zhihu.com/question/386494355](https://www.zhihu.com/question/386494355)更改设置后，编码正常<br />（一开始还以为是vector里面有乱码，还调试了半天gdb版本。。。蠢死；除了注释最好还是**别用中文**了）<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658077253655-4dd2d57f-bf17-4749-98f8-7fabe534d02c.png#clientId=u34be66d1-fad5-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=322&id=u09743cdf&margin=%5Bobject%20Object%5D&name=image.png&originHeight=532&originWidth=1206&originalType=binary&ratio=1&rotation=0&showTitle=false&size=47277&status=done&style=shadow&taskId=u2a4fdb5f-cb98-44df-ac91-e21e8036486&title=&width=730.9090486636857)

<a name="oPeEI"></a>
##### 3.18
合语法但是很危险，应当用ivec.push_back(42)
<a name="BXTzM"></a>
##### 3.19
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658111482942-7dd20e98-407b-4984-9d03-8f396cd6a8cd.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=180&id=u4321ce0e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=720&originWidth=3132&originalType=binary&ratio=1&rotation=0&showTitle=false&size=88395&status=done&style=shadow&taskId=u6a34b34a-f89d-4022-b00b-fe19e05b745&title=&width=783)<br />显然第二种方法更简便
<a name="U3kXT"></a>
##### 3.20
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658112497211-5dc3181b-8a0e-4e50-ba2c-dfd7200f62b8.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=376&id=u6ebf2b73&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1584&originWidth=2490&originalType=binary&ratio=1&rotation=0&showTitle=true&size=119179&status=done&style=shadow&taskId=u2f90d1b1-d4f6-4250-a2df-fac7274f5b3&title=%E7%9B%B8%E9%82%BB%E8%BE%93%E5%87%BA&width=590.975341796875 "相邻输出")![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658112448545-495867f4-44e0-430a-b840-1e110a3ac6e6.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=376&id=u4a07a553&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=2472&originalType=binary&ratio=1&rotation=0&showTitle=true&size=138668&status=done&style=shadow&taskId=u4cac3239-b8be-4509-8e41-ac1c9dd1bae&title=%E9%A6%96%E5%B0%BE%E8%BE%93%E5%87%BA&width=537.9923706054688 "首尾输出")
<a name="uh19Y"></a>
## 3.4 迭代器iterator介绍
类似访问容器元素的指针，有效指[start, finish]区间的迭代器，其他位置属于无效；<br />begin在首元素，end在尾元素的**后一位**；如果容器空，则begin=end；<br />end比较特殊，不指向具体元素，不能解引用或加减；<br />迭代器属于iterator和const_iterator类型，后者相当于const指针；<br />无论元素是否为常量，**cbegin**和**cend**都返回常迭代器；<br />！循环里若使用迭代器，不要改变容器容量（如添加元素），否则迭代器会失效！
<a name="jbDDk"></a>
#### 练习
<a name="HO1Ej"></a>
##### 3.23
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658113711022-d35e4856-f86e-4c96-8f78-f2dd5a30becc.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=299&id=ue5db050d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2016&originWidth=3642&originalType=binary&ratio=1&rotation=0&showTitle=false&size=184721&status=done&style=shadow&taskId=u3e70307b-032f-47e4-9ed1-fc182750623&title=&width=540.9923706054688)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658113727808-eec67feb-df14-4427-b935-b1ed81377642.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=282&id=u45b35e1e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=538&originWidth=1166&originalType=binary&ratio=1&rotation=0&showTitle=false&size=38015&status=done&style=shadow&taskId=ub5e94780-3c69-496e-8c45-a18ecf20dde&title=&width=610.6590576171875)<br />答案没有用迭代器，用的是范围for加引用
<a name="SoAPN"></a>
### 迭代器运算
it1-it2返回it2要向前移动到it1的步数（difference_type类型，可正可负），当然前提是同一容器的迭代器；<br />迭代器在前面的大，在后面的小；此处的前后、大小以end>begin为参考；
<a name="QmuBi"></a>
#### 练习
<a name="Sb5QY"></a>
##### 3.24
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658115681399-9b312dca-d308-4d94-808a-da52d913c274.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=186&id=u81271fe0&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1440&originWidth=3876&originalType=binary&ratio=1&rotation=0&showTitle=true&size=126421&status=done&style=shadow&taskId=uffadacda-7584-44a3-b287-3afb8ea9a49&title=%E8%BF%AD%E4%BB%A3%E5%99%A8%E9%87%8D%E5%81%9A%E7%9B%B8%E9%82%BB%E8%BE%93%E5%87%BA&width=501.98480224609375 "迭代器重做相邻输出")![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658115794779-f61d4bd1-0c86-47cb-8559-4b8521f0fc16.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=176&id=ube0e289d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1440&originWidth=5436&originalType=binary&ratio=1&rotation=0&showTitle=true&size=137504&status=done&style=shadow&taskId=ue488d3a3-6358-48ea-9bf5-d69c6a1cd1f&title=%E8%BF%AD%E4%BB%A3%E5%99%A8%E9%87%8D%E5%81%9A%E9%A6%96%E5%B0%BE%E8%BE%93%E5%87%BA&width=664.9658813476562 "迭代器重做首尾输出")
<a name="G7X8P"></a>
##### 3.25
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658116076112-9f3b2abe-6c0b-4ee0-855e-47c8c901ad98.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=307&id=uc0785197&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1440&originWidth=2232&originalType=binary&ratio=1&rotation=0&showTitle=false&size=137641&status=done&style=shadow&taskId=ubc94e01b-9244-45f9-852b-3a82958918f&title=&width=475.99237060546875)
<a name="tw4U9"></a>
##### 3.26
迭代器没有加法（猜想可能会导致越界，所以没有实现）
<a name="Dx22W"></a>
## 3.5 数组
数组长度是constexpr；不允许auto数组，需要指定类型；不存在引用的数组；<br />标准不允许数组拷贝
<a name="hhnuL"></a>
### 复杂数组声明
包括指针的数组、数组的指针、数组的引用<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658116438546-38abb2e2-ff1e-4ebb-9b80-9b0d11fd0877.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=112&id=u58585fb1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=185&originWidth=1087&originalType=binary&ratio=1&rotation=0&showTitle=false&size=116071&status=done&style=shadow&taskId=u02701a4d-cdfa-47f8-a660-d5c346faa07&title=&width=658.7878407109671)<br />最佳阅读顺序是从内到外然后再从右到左
<a name="lNQBU"></a>
#### 练习
<a name="i4Nu2"></a>
##### 3.27
(a)(c)(d)非法，buf_size不是常量表达式；txt_size()返回值也不是constexpr；字符串字面值末尾有'\0'，st大小至少为12
<a name="m44Sh"></a>
### 访问数组元素
数组下标为size_t类型（机器相关、无符号）
<a name="O3TJP"></a>
#### 练习
<a name="VdBzY"></a>
##### 3.30
ix=10时将出现越界
<a name="oTr36"></a>
##### 3.31
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658120758440-01e52661-d070-4b33-b2d4-9703b333e4b9.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=288&id=u8f37f3ee&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1152&originWidth=1968&originalType=binary&ratio=1&rotation=0&showTitle=false&size=71721&status=done&style=shadow&taskId=u9f3c7073-5ff1-4a6e-9213-347ed735080&title=&width=492)
<a name="L3P20"></a>
##### 3.33
不初始化的时候数组/局部变量里面是垃圾值，达不到统计分数段的目的<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658120949612-1f5ec89d-b8ba-415e-a121-81d9c1b64758.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=247&id=ue407b95b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=408&originWidth=1192&originalType=binary&ratio=1&rotation=0&showTitle=false&size=38785&status=done&style=shadow&taskId=u8a50bd32-d03f-4dc9-be47-243eed0317f&title=&width=722.4242006692482)
<a name="mgvwE"></a>
### 指针和数组
数组名在初始化表达式中自动隐式转换为首元素地址的**右值**——wiki<br />auto会把数组名认为是指针，而decltype会返回真正的数组类型

---

<a name="FJhnm"></a>
### 左值、右值
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658121437430-5200ed89-9ab1-4a0b-bb56-b310fddad2e1.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=350&id=u56105d6b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=577&originWidth=1253&originalType=binary&ratio=1&rotation=0&showTitle=true&size=98436&status=done&style=shadow&taskId=uad0af842-75a7-471f-ba7a-19990fa635f&title=%E8%A1%A5%E5%85%85%E5%B7%A6%E5%80%BC%E5%8F%B3%E5%80%BC%E7%9A%84%E6%A6%82%E5%BF%B5&width=759.3938955021542 "补充左值右值的概念")
<a name="zhkmZ"></a>
### 标准库函数begin和end
与容器成员函数类似，但不是成员函数，接收数组作参数；<br />end()-begin()返回值为ptrdiff_t类型，带符号且与机器相关；

- 数组下标可以为负数，意思是向后偏移，如：

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658122101586-7f579001-d8e1-4542-ba9d-4f7285ffad2b.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=262&id=ud89f22d6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1728&originWidth=5178&originalType=binary&ratio=1&rotation=0&showTitle=false&size=226827&status=done&style=shadow&taskId=u19050968-9ce4-413a-830d-c9ad48fa643&title=&width=784.973388671875)<br />f[-1]其实就是x[10-1]，不过这种写法不好理解

- 标准库容器下标就不可以是负数了
<a name="YOdns"></a>
#### 练习
<a name="TRL9C"></a>
##### 3.34
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658122348147-a7887c5b-bfd2-4d3e-9953-8df0c324097e.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=228&id=u2dad6b2b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=720&originWidth=2346&originalType=binary&ratio=1&rotation=0&showTitle=false&size=86425&status=done&style=shadow&taskId=u113f5eb7-b4f7-445f-934a-35b7e83e5fa&title=&width=741.9658813476562)<br />将p1指向和p2相同的位置，不会非法
<a name="wFkmf"></a>
##### 3.35
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658122448828-05eb9910-ef8c-46cc-b9d4-8d0b37ddd678.png#clientId=u40b43b2e-726a-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=519&id=ue9d4d3df&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1584&originWidth=2082&originalType=binary&ratio=1&rotation=0&showTitle=false&size=109073&status=done&style=shadow&taskId=ue967476b-32f7-497c-8213-0bea27604bc&title=&width=681.9696655273438)
<a name="hqV6d"></a>
##### 3.36
比较数组需要自己编写每个元素逐个对比的方法（包括两个数组的首尾指针）；<br />比较vector可以用封装的==操作符
<a name="PiYLw"></a>
### C风格字符串
不是一种类型；一般用指针操作<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658123978904-3cabf73c-10eb-42b0-ad9b-d388ba65c993.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=0.9751&from=paste&height=201&id=u936fe193&margin=%5Bobject%20Object%5D&name=image.png&originHeight=331&originWidth=1243&originalType=binary&ratio=1&rotation=0&showTitle=true&size=238503&status=done&style=shadow&taskId=uf88a76c6-79e0-433c-b7c0-67b4b6b9953&title=%3Ccstring%3E%E4%B8%AD%E5%AE%9A%E4%B9%89%E7%9A%84%E5%AD%97%E7%AC%A6%E4%B8%B2%E6%93%8D%E4%BD%9C&width=753 "<cstring>中定义的字符串操作")<br />这些函数都不验证字符串末尾是否有空字符，因此胡乱使用很危险

- strcmp相等返回0，p1>p2返回正数，p1<p2返回负数
- 连接、拷贝需要正确计算字符串大小，极容易出错
<a name="bqomj"></a>
#### 练习
<a name="HaojE"></a>
##### 3.37
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658124691091-13d17aa6-9b29-45dd-b608-9e6ed2ac6599.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=214&id=uadcecfb1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=462&originWidth=1172&originalType=binary&ratio=1&rotation=0&showTitle=false&size=26787&status=done&style=shadow&taskId=u4688f3e2-bdb7-4c97-850a-29a0735fbc9&title=&width=543.302978515625)<br />很明显，*cp是空时循环才会结束，而ca并不是以空字符结尾的字符串，指针会操作未知地址，所以输出的字符为垃圾值
<a name="VAitz"></a>
##### 3.40
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658124991667-357c1ef1-f64c-4ded-a282-a234767f3dd8.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=267&id=uca187bf8&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1296&originWidth=2604&originalType=binary&ratio=1&rotation=0&showTitle=false&size=176921&status=done&style=shadow&taskId=uf3801b6f-0d3a-405b-8ea6-7320d103f1a&title=&width=536.973388671875)
<a name="vDBSa"></a>
### 与旧代码的接口

1. 允许C风格字符串初始化string；甚至提供c_str()返回string的C风格字符串；<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658125273353-74094640-4d66-4a5c-92e1-f8a054e67b95.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=121&id=wd3W6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=200&originWidth=1192&originalType=binary&ratio=1&rotation=0&showTitle=false&size=180160&status=done&style=shadow&taskId=u179c592f-2ab8-408a-9c39-138e2b5e4aa&title=&width=722.4242006692482)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658125304619-3108d839-e0d5-47a4-a09f-d22c911d1ce2.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=26&id=u167e2dcf&margin=%5Bobject%20Object%5D&name=image.png&originHeight=43&originWidth=662&originalType=binary&ratio=1&rotation=0&showTitle=false&size=15666&status=done&style=shadow&taskId=ubed956c7-0d02-431e-b381-3c920bd67eb&title=&width=401.21209802268646)
2. 允许数组初始化vector<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658125346611-48d0c0a0-840f-4f7f-806d-b95cf6d1a7db.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=77&id=u5fcd2cf6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=127&originWidth=892&originalType=binary&ratio=1&rotation=0&showTitle=false&size=63189&status=done&style=shadow&taskId=ue63c1379-a3a2-424a-a41c-a453a9d1f08&title=&width=540.6060293598736)
<a name="SbowT"></a>
## 3.6 多维数组
其实是数组的数组；<br />多层范围for遍历多维数组时，除了最内层，其他层都应该声明为auto引用，否则会造成不合理的遍历指针<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658125656310-0559eae4-30c7-4ce7-b3b7-e68f101a17f1.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=78&id=u9a6a8c3b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=129&originWidth=940&originalType=binary&ratio=1&rotation=0&showTitle=false&size=60940&status=done&style=shadow&taskId=ue1007a5f-adde-4e73-bf0d-0ee4816612b&title=&width=569.6969367693736)
<a name="R6onq"></a>
#### 练习
<a name="UV6aS"></a>
##### 3.43
<a name="L9sGq"></a>
##### ![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658131362235-045be88d-ef33-4c76-8ebd-b3a8d8ad1b71.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=1800&id=ufd564587&margin=%5Bobject%20Object%5D&name=image.png&originHeight=3600&originWidth=7260&originalType=binary&ratio=1&rotation=0&showTitle=false&size=462663&status=done&style=shadow&taskId=ub242237f-b25d-46db-9f68-6adcb34a755&title=&width=3630)
<a name="dai2D"></a>
##### 3.44
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658131550427-649e3da2-6748-4e6d-a9aa-38b0edb9a36f.png#clientId=u477f4f71-72dd-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=2232&id=u8e7d1da5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=4464&originWidth=7260&originalType=binary&ratio=1&rotation=0&showTitle=false&size=552253&status=done&style=shadow&taskId=ue19c1719-77c2-4b27-8fc1-f7d2795c313&title=&width=3630)<br />改动不大，主要是外层循环看起来简洁一些
<a name="vPNAm"></a>
##### 3.45
把int_array换成auto，尤其是范围for会更简洁
<a name="cFI6b"></a>
# 第4章 表达式
<a name="w8zDl"></a>
## 4.1 基础
<a name="kWGpo"></a>
### 左值右值
左值可以放在=左边，但const对象不能作为左值；<br />有些表达式结果为对象，但却是右值；<br />**总结：	**对象右值是内容，左值是内存中的位置；<br />左值可以代替右值，反之则不行；<br />左值当右值用的时候，用的是内容

- =左边需要左值，且返回左值
- &作用于左值，却返回右值（地址）
- []和*都返回左值
- ++、--作用于左值，前置的返回也是左值
- decltype(expression)，如果表达式是左值（非变量）则返回引用<br />是右值则正常返回操作符的结果类型

---

<a name="Gb20b"></a>
### &操作符的结果是指针右值
很困惑的一点是，取地址运算符&返回指针右值，猜测也是这样，不然不会有int *p=&i的写法；<br />在标准中找到&的定义<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658134898949-d25f554e-4f4f-4ad6-b1e2-baadd7f8dbdd.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=371&id=u4c648095&margin=%5Bobject%20Object%5D&name=image.png&originHeight=612&originWidth=1890&originalType=binary&ratio=1&rotation=0&showTitle=false&size=133708&status=done&style=shadow&taskId=ubbdd199a-9540-4335-9683-582d454856c&title=&width=1145.4544792490597)<br />可以看到确实是返回指针类型，那以后记住就好

---

<a name="aLY9d"></a>
### 优先级和结合律
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658135162505-012bab26-ccab-4d3a-86c8-b5c0fc8a1c8e.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=760&id=u425afe56&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1192&originWidth=1028&originalType=binary&ratio=1&rotation=0&showTitle=false&size=505402&status=done&style=shadow&taskId=u8aa2b3e8-beb0-44df-9fb6-ea2cb2b1aeb&title=&width=655.0302734375)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658135232162-e9df17e9-faa4-4d60-bf69-6f7e398c412e.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=1096&id=ube22f3cc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1238&originWidth=744&originalType=binary&ratio=1&rotation=0&showTitle=false&size=414713&status=done&style=shadow&taskId=u0fddb8be-92b1-4653-9132-31b2418f9b5&title=&width=658.9071655273438)

- 表中靠前的优先级高，同一组内优先级相同
- 算术运算符和成员访问都是左结合，还有逗号，其他大多都是右结合
<a name="j3DLV"></a>
#### 练习
<a name="knxyu"></a>
##### 4.1
结果应为105
<a name="qQMxu"></a>
##### 4.2
在vec.begin()两边加括号即可
<a name="PAO7V"></a>
### 求值顺序
和优先级、结合律无关；<br />如![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658135555870-988ab2ca-9d53-48a3-a16a-c5664a6bd335.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=40&id=ubc83994b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=66&originWidth=285&originalType=binary&ratio=1&rotation=0&showTitle=false&size=9062&status=done&style=shadow&taskId=u66bd8643-3e5a-4ec2-a03c-76fa4698c91&title=&width=172.7272627439058)这样的表达式<br />函数调用顺序一般由编译器决定
<a name="eYXBi"></a>
## 4.2 算术运算符

- 对象和结果都是右值（当然前面提过，左值可以代替右值）
- 会进行隐式类型转换<br />尤其是bool会转成int，因此不要用于参与运算<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658136453165-e195e817-42ff-4524-872e-e02a04855095.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=58&id=u6b3411c4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=288&originWidth=1392&originalType=binary&ratio=1&rotation=0&showTitle=false&size=23260&status=done&style=shadow&taskId=uc1db001b-1768-4eb5-bd43-3582817e3d1&title=&width=281.6325378417969)
- 新标准商一律舍弃小数部分<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658136666151-5e39a4b4-d3cf-4f09-9541-5985790046b6.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=34&id=ubcfb5ce5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=144&originWidth=1914&originalType=binary&ratio=1&rotation=0&showTitle=false&size=27021&status=done&style=shadow&taskId=u5a7a08d1-3a30-46ad-8d33-f22b85c3a47&title=&width=447.98095703125)
- m - (m/n) * n = m % n<br />按照这个方程求模；如果m%n不为0，那么结果符号和m相同
<a name="UvsvV"></a>
#### 练习
<a name="q9Lty"></a>
##### 4.4
结果应为91
<a name="BveS3"></a>
##### 4.5
(a)-86；	(b)-18；<br />(c)0;	(d)-2
<a name="dhBwT"></a>
##### 4.6
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658147029711-b075e06d-db92-47d1-a6f0-fb59074f7e4a.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=91&id=u3d1de922&margin=%5Bobject%20Object%5D&name=image.png&originHeight=432&originWidth=3126&originalType=binary&ratio=1&rotation=0&showTitle=false&size=47022&status=done&style=shadow&taskId=u1d8771b5-be01-4a5b-add3-6f503ebb375&title=&width=661.9715576171875)
<a name="ydeX5"></a>
##### 4.7
当计算的结果超出该类型所能表示的范围时就会产生溢出。<br />这里仅给一个例子，无符号数0强行减一会变成unsigned int的模<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658151330379-b4e7ad72-392c-4767-9e2d-8f4ac338d202.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=108&id=u6b88789b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=486&originWidth=1590&originalType=binary&ratio=1&rotation=0&showTitle=false&size=28426&status=done&style=shadow&taskId=u5277e990-3ddd-4c06-aadf-5a81790c873&title=&width=353.63629150390625)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658151350225-aa6e0543-cda4-4c77-a97b-fe5fbc289717.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=123&id=uc1f65876&margin=%5Bobject%20Object%5D&name=image.png&originHeight=203&originWidth=632&originalType=binary&ratio=1&rotation=0&showTitle=false&size=19439&status=done&style=shadow&taskId=ua942a651-506e-4b53-b260-2187325e9df&title=&width=383.030280891749)
<a name="gFW3L"></a>
## 4.3 逻辑和关系运算符
运算对象和返回值都是右值；<br />||和&&出现短路求值的现象，当第一个开关断开时，后面的表达式不再进行计算；
<a name="j9FA2"></a>
#### 练习
<a name="cBx95"></a>
##### 4.9
cp为字符串字面值的地址，不会为0；<br />*cp是'H'字符，也不为0；<br />所以此条件为true
<a name="L2HOn"></a>
##### 4.10
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658152539149-a14ac8e3-28c4-4e67-bf7a-a3965aa0a793.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=162&id=u6d84853c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=648&originWidth=1770&originalType=binary&ratio=1&rotation=0&showTitle=false&size=38379&status=done&style=shadow&taskId=u0258d918-54eb-4579-9b65-cac55074eba&title=&width=443)
<a name="t03QI"></a>
##### 4.12
大于小于优先级大于判等；<br />j<k结果为true或false，和int判等时转换为1或0；也就是判断i是否等于1或0
<a name="m6T8r"></a>
## 4.4 赋值运算符
=左侧是可修改的左值，结果是左侧类型的左值；<br />右侧对象会转成左侧类型；<br />允许列表初始化<br />左侧为内置类型时，列表只能包含一个值，且不可以往小类型转换；<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658153330550-5878b7a5-29c5-43a4-89ed-008e8679e42f.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=58&id=u0487fa10&margin=%5Bobject%20Object%5D&name=image.png&originHeight=95&originWidth=759&originalType=binary&ratio=1&rotation=0&showTitle=false&size=9146&status=done&style=shadow&taskId=u7a1b87d9-c36c-474f-be7c-9f59fbb67cb&title=&width=459.99997341271757)<br />=优先级非常低，一般加个括号；<br />复合赋值只计算一次，在重载操作符和操作类对象时开销较小；
<a name="qxnxd"></a>
#### 练习
<a name="DFKvk"></a>
##### 4.15——解惑
ival = pi一部分非法，int*不可以用来初始化int<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658154528825-de057851-e218-4a63-8543-5406242ec775.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=260&id=ub2d07507&margin=%5Bobject%20Object%5D&name=image.png&originHeight=429&originWidth=1817&originalType=binary&ratio=1&rotation=0&showTitle=false&size=46129&status=done&style=shadow&taskId=ue15b5f25-4420-44e4-a09a-106e4c68031&title=&width=1101.2120575637784)<br />标准对=运算符有解释，右侧必须可以隐式转换为左侧<br />pi的值为16进制地址，可能这是无法隐式转换的原因<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658154807067-001ef1cc-cc28-4a77-aa75-6c3989e1ec5f.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=61&id=ucd08f06d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=100&originWidth=1709&originalType=binary&ratio=1&rotation=0&showTitle=false&size=19866&status=done&style=shadow&taskId=u84dcf319-0a22-4d78-8c5e-c9c1a4c559b&title=&width=1035.7575158924035)<br />地址太长转为int损失了精度，经测试转为较大的long long类型可以通过<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658154892390-6668f199-9db3-433c-adcb-5c9719040a69.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=99&id=ud4aba83e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=486&originWidth=1830&originalType=binary&ratio=1&rotation=0&showTitle=false&size=42464&status=done&style=shadow&taskId=uae996630-c61d-4cee-ab34-9f3c82b0a54&title=&width=371.0738220214844)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658154906533-32b3fc45-3bb0-4788-8105-053e7c9caddb.png#clientId=ubd509992-3aaf-4&crop=0&crop=0.0628&crop=1&crop=1&from=paste&height=112&id=u306045b5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=184&originWidth=1189&originalType=binary&ratio=1&rotation=0&showTitle=false&size=21725&status=done&style=shadow&taskId=u2c302211-fecd-4400-bd4d-662d8257abb&title=&width=721)
<a name="jMtFu"></a>
## 4.5 递增和递减运算符
作用于左值，前置返回对象本身左值，后置返回对象原值副本的右值；<br />一般不要用后置版本，除非需要同时递增和使用原值；后置++优先于解引用*
<a name="dUE1H"></a>
#### 练习
<a name="CHF79"></a>
##### 4.19
(c)应修改，没有规定<=两边求值顺序
<a name="AipUi"></a>
## 4.6 成员访问运算符
*低于点，最好加括号；

- ->作用于对象指针，返回左值
- 点：返回成员所属对象的左右值类型
<a name="F0yeN"></a>
#### 练习
<a name="GAswj"></a>
##### 4.20
(b)(c)(e)不合法，string没有自增操作，而且(c)这里不是想使用迭代器的成员函数empty()，应该加括号
<a name="ICEMW"></a>
## 4.7 条件运算符
即condition？expr1：expr2；<br />当两个表达式都是左值或可以转换成同一种左值时，返回左值；否则返回右值；<br />最好别嵌套；<br />优先级很低，仅高于=，记得加括号；<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658158042183-a0635b48-b2e6-44de-8eeb-635cd41ec3c0.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=81&id=u873eec12&margin=%5Bobject%20Object%5D&name=image.png&originHeight=133&originWidth=1174&originalType=binary&ratio=1&rotation=0&showTitle=false&size=86546&status=done&style=shadow&taskId=u9699ebfe-49bc-4466-ae9d-3e3a0488e72&title=&width=711.5151103906857)
<a name="n4ygc"></a>
#### 练习
<a name="t0O1h"></a>
###### 4.21
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658158208470-b07cf796-3b72-4a12-bdcf-86d45754abdd.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=215&id=ufff65562&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1134&originWidth=2442&originalType=binary&ratio=1&rotation=0&showTitle=false&size=110164&status=done&style=shadow&taskId=uaf4c6805-bc53-43b8-8a09-d904d19316f&title=&width=462.9942626953125)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658158223156-88b3b0c8-ab1b-42bb-b496-6b377a238182.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=188&id=VJVyM&margin=%5Bobject%20Object%5D&name=image.png&originHeight=376&originWidth=1137&originalType=binary&ratio=1&rotation=0&showTitle=false&size=28762&status=done&style=shadow&taskId=u77448e67-233b-4e80-b6bb-bff7a8f8e1d&title=&width=569)
<a name="U4M06"></a>
##### 4.22
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658158886295-af272e89-593d-46c8-945f-1383bb927c92.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=309&id=uff337022&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2430&originWidth=6768&originalType=binary&ratio=1&rotation=0&showTitle=false&size=233412&status=done&style=shadow&taskId=uf0dd1a3b-060e-422f-891a-ebfb74363ab&title=&width=860.9715576171875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658158904703-22393f36-d8d7-4922-bcf9-e04e81024a3f.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=208&id=u240b833e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=344&originWidth=197&originalType=binary&ratio=1&rotation=0&showTitle=false&size=12623&status=done&style=shadow&taskId=u583f1592-84c0-4df9-9a80-8bb2f84f44f&title=&width=119.39393249315594)<br />if版本就不写了，显然是if容易理解
<a name="eUtxN"></a>
##### 4.23
+后面加括号即可，代码功能是如果词尾没有s加上s
<a name="LQt1q"></a>
## 4.8 位运算符
作用于整形对象或bitset；<br />尽量只用于无符号类型；<br />^异或：不同为1，相同为0；

- <<左移在右侧补0；>>右移在左侧补符号位或0；

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658159383207-1e18be8c-2054-456d-8c2e-8a5981a21890.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=304&id=ubac6a3a4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=502&originWidth=1888&originalType=binary&ratio=1&rotation=0&showTitle=false&size=63559&status=done&style=shadow&taskId=u4615b38b-8a5b-4c85-bf48-e34c0917516&title=&width=1144.242358106997)
<a name="jtbti"></a>
#### 练习
<a name="TVYMj"></a>
##### 4.25
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658159745303-e4bec44e-b9ab-42a5-8753-a40acac54ba2.png#clientId=ubd509992-3aaf-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=206&id=u143b2579&margin=%5Bobject%20Object%5D&name=image.png&originHeight=810&originWidth=1956&originalType=binary&ratio=1&rotation=0&showTitle=false&size=99172&status=done&style=shadow&taskId=u888d6755-118b-44fe-aaf5-bc0c1cc9b4e&title=&width=496.973388671875)
<a name="PrifB"></a>
##### 4.27
(a)3		(b)7<br />(c)true	(d)true
<a name="ZPePx"></a>
## 4.9 sizeof运算符
返回操作对象所占字节数，返回**constexpr **size_t类型

- sizeof(type)
- sizeof expr返回表达式结果类型的大小

sizeof结果还有些规定：<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658195112468-6a7d8fc9-f8c6-4356-ad12-aedf524a9c42.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=158&id=u382d0365&margin=%5Bobject%20Object%5D&name=image.png&originHeight=261&originWidth=1199&originalType=binary&ratio=1&rotation=0&showTitle=false&size=171853&status=done&style=shadow&taskId=u2d65b0d8-5cf7-4d69-bab8-37efbe9a2bf&title=&width=726.6666246664669)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658195119285-7fe16393-cb5f-4aef-8e93-913ecc3bf9e8.png#clientId=uaa3d56e2-d9b7-4&crop=0.0145&crop=0&crop=1&crop=1&from=paste&height=160&id=u4149ff0e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=268&originWidth=1251&originalType=binary&ratio=1&rotation=0&showTitle=false&size=195205&status=done&style=shadow&taskId=ubb859d26-e1b8-46b3-a86b-4142a06ba18&title=&width=747)
<a name="Fm2xO"></a>
#### 练习
<a name="A02QF"></a>
##### 4.28
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658199685257-c1e41bc5-655f-4ade-bda4-9378f7b33c47.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=310&id=u7da44193&margin=%5Bobject%20Object%5D&name=image.png&originHeight=511&originWidth=377&originalType=binary&ratio=1&rotation=0&showTitle=false&size=42940&status=done&style=shadow&taskId=u198a645a-43d6-470f-bb83-4790426a262&title=&width=228.48483527878065)
<a name="YlpG5"></a>
##### 4.29
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658202505860-2fc3ab14-65fc-41a7-b95e-16c78f468aa7.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=50&id=u7d3e6059&margin=%5Bobject%20Object%5D&name=image.png&originHeight=83&originWidth=622&originalType=binary&ratio=1&rotation=0&showTitle=false&size=22979&status=done&style=shadow&taskId=ubec5c485-3d1a-4b75-a4b3-268ca78d0e1&title=&width=376.9696751814365)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658202582545-44f1cb61-5d87-4a3f-9bd7-2bd10fb4aa4d.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=125&id=u2392e42d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=648&originWidth=4578&originalType=binary&ratio=1&rotation=0&showTitle=false&size=158005&status=done&style=shadow&taskId=ud4bf1d20-f97e-421c-a0d9-b7a93f01637&title=&width=880.973388671875)<br />不是像答案说的未定义
<a name="lNlRt"></a>
##### 4.30
sizeof优先级高于算术运算符，(a)(c)在运算符左边加括号即可
<a name="ZtVii"></a>
## 4.10 逗号运算符
求值顺序从左到右，结果是最右边表达式的值（无论左右）
<a name="rydW4"></a>
#### 练习
<a name="S8rcg"></a>
##### 4.31
此处变为后置即可，由于是for循环的第三个迭代语句，不会产生副作用
<a name="pC4Bg"></a>
##### 4.32
含义即遍历数组：ix与size组合和ptr与ia组合一样，都是确定边界的作用
<a name="r7CSy"></a>
##### 4.33
(someValue ? ((++x), (++y)) : (--x)), (--y)<br />前置自增自减优先级最高，先加一层括号；<br />？：优先级高于逗号，逗号前再加一层括号<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658203581661-673235a3-1884-4af5-863b-156e6aaf7ee5.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=77&id=u95016d67&margin=%5Bobject%20Object%5D&name=image.png&originHeight=486&originWidth=3828&originalType=binary&ratio=1&rotation=0&showTitle=false&size=87072&status=done&style=shadow&taskId=u86784b81-ac78-42ea-8691-42c29d80877&title=&width=603.973388671875)
<a name="YAMer"></a>
## 4.11 类型转换
<a name="qykON"></a>
### 隐式转换——算术类型<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658214004325-02910923-ea16-4aab-8ca8-414bfaf3febf.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=230&id=u68f0122a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=380&originWidth=1221&originalType=binary&ratio=1&rotation=0&showTitle=false&size=271801&status=done&style=shadow&taskId=ub81c1770-2407-4015-a243-7b0060a739d&title=&width=739.9999572291543)

- 小整数如果可能都提升为int，否则提升为unsigned int
- 无符号和带符号在一起转换成范围更大的类型
<a name="AKOWB"></a>
#### 练习
<a name="jLC3F"></a>
##### 4.34
（a）float转int<br />（b）int转float，float转double<br />（c）char转int，int转double
<a name="doFVG"></a>
##### 4.35
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658218373863-74fc9f27-749b-4d32-8c30-323b59695af9.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=140&id=u6a0121b2&margin=%5Bobject%20Object%5D&name=image.png&originHeight=648&originWidth=1794&originalType=binary&ratio=1&rotation=0&showTitle=true&size=69020&status=done&style=shadow&taskId=u10483fa5-a9f4-4cb3-b414-94e00f5ee05&title=%EF%BC%88a%EF%BC%89&width=387.272705078125 "（a）")![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658218573745-759e0b90-7c42-484f-bf64-79b3fde908a3.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=170&id=uc9ad3b7e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=810&originWidth=2256&originalType=binary&ratio=1&rotation=0&showTitle=true&size=124259&status=done&style=shadow&taskId=uca82d896-d139-40db-bfde-ed06b4f03a4&title=%EF%BC%88b%EF%BC%89&width=472.96966552734375 "（b）")<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658218759623-abf202af-9bad-4831-88ad-7b4a4ba000e4.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=203&id=u0d88a7d9&margin=%5Bobject%20Object%5D&name=image.png&originHeight=972&originWidth=1872&originalType=binary&ratio=1&rotation=0&showTitle=true&size=109399&status=done&style=shadow&taskId=u63afe3e5-0f9e-410f-8998-50714c9c81c&title=%EF%BC%88c%EF%BC%89&width=390.9924011230469 "（c）")![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658219009074-07b70c49-06a4-4736-b9da-f2fa20f100f4.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=227&id=u1e13e4eb&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1458&originWidth=2724&originalType=binary&ratio=1&rotation=0&showTitle=true&size=183958&status=done&style=shadow&taskId=u33c55dd9-afe2-4c12-b9d3-87ad605cba5&title=%EF%BC%88d%EF%BC%89&width=424.973388671875 "（d）")<br />每小段都进行了两三次隐式转换
<a name="P5A7f"></a>
### 其他隐式转换

- **数组转换成指针**<br />decltype、&、sizeof、typeid例外
- **指针转换<br />**0、nullptr能转换成任意指针；<br />非const指针可以转换为void*；<br />非空指针可以转换为const void*
- 类定义的转换<br />如cin转换为bool
<a name="UOq9o"></a>
### 显式转换
格式：cast-name <type> (expression)

- cast有四种：<br />static_cast 、 dynamic_cast、const_cast、reinterpret_cast
- type是引用时结果是左值？<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658220145709-f36a15e9-d630-48ac-af7a-a8b1b09afee8.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=93&id=u981690b8&margin=%5Bobject%20Object%5D&name=image.png&originHeight=154&originWidth=1615&originalType=binary&ratio=1&rotation=0&showTitle=false&size=31730&status=done&style=shadow&taskId=ucdd2135b-27f2-4c13-a786-de6c5d086b6&title=&width=978.7878222154662)

---

1. static_cast本质上是传统c语言强制转换的替代品<br />不包含底层const都可以使用<br />编译通过，自己负责精度损失
2. const_cast改变对象的底层const<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658221727820-5c963dcf-180f-4bb8-b8d1-4adcdf604e02.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=122&id=u5dacb2ee&margin=%5Bobject%20Object%5D&name=image.png&originHeight=486&originWidth=2346&originalType=binary&ratio=1&rotation=0&showTitle=false&size=87552&status=done&style=shadow&taskId=u639aefac-4706-4f15-b8b7-ff2f5e0b687&title=&width=587)消去j底层const<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658221935872-0e4cd2c4-58f2-40de-a218-0b611ddc5b6d.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=122&id=ua9bcccfe&margin=%5Bobject%20Object%5D&name=image.png&originHeight=486&originWidth=2562&originalType=binary&ratio=1&rotation=0&showTitle=false&size=83653&status=done&style=shadow&taskId=ua9a61dfb-7e4b-4882-82f7-21e40ef1ad5&title=&width=641)加上x底层const
3. reinterpret_cast<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658222580156-fa5f9bd8-3473-4877-b628-3580382eb4f2.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=145&id=SuG4B&margin=%5Bobject%20Object%5D&name=image.png&originHeight=810&originWidth=3846&originalType=binary&ratio=1&rotation=0&showTitle=false&size=146446&status=done&style=shadow&taskId=ua314a727-8d69-4b0e-83a2-729bab60e2c&title=&width=688.973388671875)reinterpret_cast的例子
<a name="txGWQ"></a>
### 补充——ASCII码对照表
![网上ASCII对照表](https://cdn.nlark.com/yuque/0/2022/jpeg/21578825/1658222548847-61de5965-8a9c-400a-9c17-6cbc22314942.jpeg#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&id=u780f2ec4&margin=%5Bobject%20Object%5D&originHeight=687&originWidth=1146&originalType=url&ratio=1&rotation=0&showTitle=true&status=done&style=shadow&taskId=u0f3b682f-1dd9-4b02-8d79-75962c1820f&title=%E7%BD%91%E4%B8%8AASCII%E5%AF%B9%E7%85%A7%E8%A1%A8 "网上ASCII对照表")
<a name="NgZBK"></a>
# 第5章 语句
<a name="Yr5yj"></a>
## 5.3 条件语句
if嵌套时会发生if多于else的情况，C++规定**else与离他最近且未被匹配的if匹配**——悬垂else；<br />switch-case中的case必须是整型常量表达式；<br />不可以在一个被跳过的case中定义将会使用的变量
<a name="hrCUM"></a>
#### 练习
cin >> std::noskipws >> ch这种输入方式可以让输入流不跳过空白字符
<a name="XxdZh"></a>
##### 5.13
(c)
```cpp
unsigned evenCnt = 0, oddCnt = 0;
int digit = get_num() % 10;
switch (digit) {
	case 1: case 3: case 5: case 7: case 9://不可以写成case 1,3,5,7,9:
        oddcnt++;
        break;
    case 2: case 4: case 6: case 8: case 0:
        evencnt++;
        break;
}
```
<a name="wFgd5"></a>
## 5.4 迭代语句
<a name="NGQNR"></a>
### while语句
<a name="CQHTk"></a>
#### 练习
<a name="c9B2L"></a>
##### 5.14
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658241432123-5d4b7ab4-4260-45fa-929f-9505fc8cfbd2.png#clientId=uaa3d56e2-d9b7-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=219&id=uba831d06&margin=%5Bobject%20Object%5D&name=image.png&originHeight=361&originWidth=1346&originalType=binary&ratio=1&rotation=0&showTitle=false&size=306041&status=done&style=shadow&taskId=u1653bf89-073c-4946-bfa0-538e1707084&title=&width=815.7575286080604)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658291454617-a457398d-b378-4d79-9406-eb24297a1121.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=581&id=ucc823b0d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=3564&originWidth=4998&originalType=binary&ratio=1&rotation=0&showTitle=false&size=445425&status=done&style=shadow&taskId=u39577a06-b30c-410a-8ce4-053c727f5cf&title=&width=814.9715576171875)<br />多写这种没有使用高级数据结构的代码有助于培养机器思维
<a name="QCImb"></a>
### 传统for循环
for循环第一部分只能声明多个相同类型的变量
<a name="f3COw"></a>
#### 练习
<a name="NsnK4"></a>
##### 5.17
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658294334147-9d69a533-9342-4a02-a384-d19de5001635.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=245&id=u05efef87&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1650&originWidth=3360&originalType=binary&ratio=1&rotation=0&showTitle=false&size=148908&status=done&style=shadow&taskId=u4e5f094b-2efe-4ccd-bbab-1b23be10803&title=&width=498.99993896484375)
<a name="eTrKz"></a>
### 范围for语句
遍历的对象必须可以返回begin和end迭代器；<br />如果更改容器元素个数，范围for预存的end()将失效
<a name="BT6XU"></a>
#### 练习
<a name="yIotD"></a>
##### 5.19
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658294758374-5571757d-1f16-4fdb-abb4-d59cb32030ca.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=267&id=u58a8a201&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1650&originWidth=3012&originalType=binary&ratio=1&rotation=0&showTitle=false&size=136646&status=done&style=shadow&taskId=u7fa5fe0c-2a78-40f3-90cd-fd84db305ce&title=&width=486.99237060546875)
<a name="M051g"></a>
## 5.5 跳转语句
<a name="s1v9n"></a>
#### 练习
<a name="z3BPn"></a>
##### 5.20
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658295303159-881430d1-9d53-4a9e-a78e-e79fb4cd21a5.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=435&id=u80a32416&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2400&originWidth=2664&originalType=binary&ratio=1&rotation=0&showTitle=false&size=172139&status=done&style=shadow&taskId=u41babf29-d336-469b-9a32-ab34a3e507c&title=&width=482.9677734375)
<a name="B6Jvn"></a>
##### 5.21
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658295508752-cd11f366-0724-434b-a6f7-fb56c79f1ec4.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=391&id=u7db853f3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2400&originWidth=2946&originalType=binary&ratio=1&rotation=0&showTitle=false&size=190761&status=done&style=shadow&taskId=u1f4aafcf-8e93-48eb-a4e3-2d290a63637&title=&width=479.973388671875)
<a name="hB7Ln"></a>
##### 5.22
```cpp
do{
	int sz=get_size();
}while(sz<=0);
```
<a name="ntjrz"></a>
## 5.6 try语句块和异常处理
runtime_error对象的what()返回异常对象的初始化字符串
<a name="GaWrm"></a>
### 标准异常
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658296088238-5fc5cd01-a8b1-4aa7-8029-8eb2a199d344.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=599&id=uab61584d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=988&originWidth=1300&originalType=binary&ratio=1&rotation=0&showTitle=false&size=639664&status=done&style=shadow&taskId=u7a72b6ca-f87c-49a0-b8d9-14e7723aaf8&title=&width=787.8787423406229)

- exception、bad_alloc、bad_cast对象只能默认初始化
- 其他异常对象必须用字符串初始化

如果初始化了，what（）返回初始化字符串；否则返回值由编译器决定
<a name="Yem9N"></a>
#### 练习
<a name="ucwy5"></a>
##### 5.23
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658297768723-f1a226aa-954e-4378-8f1f-f1274e66b868.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=90&id=u0d3487b4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=450&originWidth=1626&originalType=binary&ratio=1&rotation=0&showTitle=false&size=33642&status=done&style=shadow&taskId=u75679937-9caa-4616-80ee-d29335b87dc&title=&width=323.4544677734375)
<a name="HpwMp"></a>
##### 5.24
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658298077806-fa4f7981-3a45-47b6-915a-b419b0c339d7.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=153&id=uf2cc4cbf&margin=%5Bobject%20Object%5D&name=image.png&originHeight=750&originWidth=2382&originalType=binary&ratio=1&rotation=0&showTitle=false&size=71445&status=done&style=shadow&taskId=uad1372d4-7639-4932-986b-d433f5942ba&title=&width=485.973388671875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658298099930-a6f789cc-77e5-4c0e-ba5b-ad0dc707ca0b.png#clientId=ue02841fc-6b51-4&crop=0&crop=0.0333&crop=1&crop=1&from=paste&height=180&id=u334664ec&margin=%5Bobject%20Object%5D&name=image.png&originHeight=359&originWidth=1136&originalType=binary&ratio=1&rotation=0&showTitle=false&size=37320&status=done&style=shadow&taskId=ufdd0e0e3-b04b-4e55-b687-0eea4aa4445&title=&width=570)
<a name="ylhx0"></a>
##### 5.25
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658299107774-e719a6f2-4832-483c-9d69-7c69a5633953.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=342&id=udb6a883c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2250&originWidth=3246&originalType=binary&ratio=1&rotation=0&showTitle=false&size=196952&status=done&style=shadow&taskId=u33a40d8d-15d4-4b62-9370-fcadf1f7eab&title=&width=493.998046875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658299128962-68ea5248-e51a-447b-a529-739d217da534.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=164&id=u4860622f&margin=%5Bobject%20Object%5D&name=image.png&originHeight=271&originWidth=375&originalType=binary&ratio=1&rotation=0&showTitle=false&size=13215&status=done&style=shadow&taskId=u75e08a3d-14cd-4a8b-847c-eb38822bb05&title=&width=227.27271413671815)<br />throw后面的语句不会执行；<br />try里面还是要写throw；<br />catch尽量写异常引用，不用复制异常对象
<a name="tG1Z9"></a>
# 第6章 函数
<a name="Yuh2M"></a>
## 6.1 函数基础
()叫调用运算符；<br />返回值不能是数组或函数，但可以是指针；
<a name="fixG4"></a>
#### 练习
<a name="bZESs"></a>
##### 6.4
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658299769912-e78ec936-39c2-48f2-9d77-54a416e4538f.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=319&id=u413e69a0&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1650&originWidth=1728&originalType=binary&ratio=1&rotation=0&showTitle=false&size=93935&status=done&style=shadow&taskId=u84a3317c-0d3e-48df-a661-8807d4c17a1&title=&width=334.272705078125)提前写了个递归。。
<a name="MSpQM"></a>
##### 6.5
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658300017144-58bc3cae-7691-4256-95d6-608c07e7fba6.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=373&id=u8f51a338&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1800&originWidth=1614&originalType=binary&ratio=1&rotation=0&showTitle=false&size=91678&status=done&style=shadow&taskId=u57653510-230a-43da-9067-4ee2bc356f9&title=&width=334.1723327636719)
<a name="NgCSB"></a>
##### 6.6
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658300569454-1e121d1f-2028-452c-b51f-b62422d69915.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=341&id=uccf11cd6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1800&originWidth=2928&originalType=binary&ratio=1&rotation=0&showTitle=false&size=194409&status=done&style=shadow&taskId=u4f736d94-9c2d-45db-9e03-90803efc698&title=&width=553.9639892578125)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658300594734-bbe2a9ed-e7d6-4eb1-9a19-14d478af66bb.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=82&id=u33757463&margin=%5Bobject%20Object%5D&name=image.png&originHeight=136&originWidth=405&originalType=binary&ratio=1&rotation=0&showTitle=false&size=15728&status=done&style=shadow&taskId=ud97b0429-8183-465c-b390-3f3b77a33e6&title=&width=245.45453126765563)<br />可见没写return也可以编译通过，但返回值是垃圾值
<a name="L3RUl"></a>
##### 6.7
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658300720993-41a20c06-1470-40f4-b249-910952afe375.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=312&id=u90a44a09&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1500&originWidth=1446&originalType=binary&ratio=1&rotation=0&showTitle=false&size=92124&status=done&style=shadow&taskId=u0379f1db-a2be-41b8-8868-4388d9b6daa&title=&width=300.35601806640625)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658300737857-ba53bd7f-8103-49b4-8198-ca893c026b44.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=102&id=ud7975642&margin=%5Bobject%20Object%5D&name=image.png&originHeight=168&originWidth=620&originalType=binary&ratio=1&rotation=0&showTitle=false&size=16984&status=done&style=shadow&taskId=ue86098cd-56b8-476f-886b-91e98c71a34&title=&width=375.75755403937404)
<a name="pU0g3"></a>
##### 6.10
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658301112823-88f9e02c-0a94-4753-8b60-be60ce4b0c2d.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=287&id=u1ba95a0a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1650&originWidth=2838&originalType=binary&ratio=1&rotation=0&showTitle=false&size=111612&status=done&style=shadow&taskId=u78e745be-e5b2-4981-8666-cae6ea7128a&title=&width=493.96966552734375)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658301133317-e75ebe55-c942-4415-abbc-098d83783f29.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=72&id=ub4c19039&margin=%5Bobject%20Object%5D&name=image.png&originHeight=118&originWidth=426&originalType=binary&ratio=1&rotation=0&showTitle=false&size=10037&status=done&style=shadow&taskId=u65e61659-f29d-4e07-b57b-304de4a6cc4&title=&width=258.18180325931183)
<a name="d0fWP"></a>
## 6.2 参数传递
总结使用引用传值的场景和优势：

1. 直接使用参数对象，无需拷贝，尤其是大类型或不支持拷贝的类型
2. 返回多个参数可以在参数中加引用影响外部变量
<a name="d8IvZ"></a>
#### 练习
<a name="Ew17z"></a>
##### 6.15
<a name="JifOU"></a>
##### ![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658303864583-eb0bd6ad-600a-4670-a743-d07266ce5fe5.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=305&id=ueef0b0f2&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1950&originWidth=4692&originalType=binary&ratio=1&rotation=0&showTitle=false&size=196776&status=done&style=shadow&taskId=uccc7d26b-8eab-48ff-9708-af4c75620e3&title=&width=733.9677734375)
不需要改变s引用的对象所以s最好是const引用，而occurs用来存储字符位置，所以不能是const引用；<br />s为引用可以避免拷贝（尤其是s过大的时候），occurs是引用或指针才可以更改实参（引用更简洁），c不需要声明为引用；<br />s如果为普通引用则可能更改实参（不希望看到），occurs需要修改值不能为const引用
<a name="h0Z4i"></a>
##### 6.16
参数改为const引用：<br />此函数不修改参数，最好是const引用<br />此函数可以接收const string，但普通引用不可以引用const对象，所以此时必须是const
<a name="DuTVu"></a>
##### 6.17
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658304761511-e85b2420-d8f8-4248-a43f-f07b97a6899a.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=399&id=u54dfda18&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2850&originWidth=3624&originalType=binary&ratio=1&rotation=0&showTitle=false&size=278763&status=done&style=shadow&taskId=u2d96a2a7-eee8-432a-8121-9914d82342c&title=&width=507.96209716796875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658304781903-00286e1a-394e-43dc-8d32-40f86b4bccfb.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=38&id=u6b5f10e4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=62&originWidth=113&originalType=binary&ratio=1&rotation=0&showTitle=false&size=2036&status=done&style=shadow&taskId=ub055ad54-6d56-4521-b45d-3034ba56cab&title=&width=68.48484452653108)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658305091303-8dc8f164-e7ac-4dae-8926-da4a96c7b1f5.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=223&id=u366ca212&margin=%5Bobject%20Object%5D&name=image.png&originHeight=368&originWidth=1310&originalType=binary&ratio=1&rotation=0&showTitle=false&size=348580&status=done&style=shadow&taskId=u67a2732f-8209-4154-96e2-3a39481cb5a&title=&width=793.9393480509355)
<a name="CksI2"></a>
### 数组形参
由于数组名字被当作指针，数组长度函数未知，即使明确指出，编译器也只检查类型；<br />管理方法有以下几种：

- C风格字符串碰到空字符结束
- 标准库启发：传递首指针和尾后指针
- 直接传入数组大小<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658305309415-5713b4bb-28ff-4598-8f6b-18eff696e89d.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=121&id=u3e8c0f80&margin=%5Bobject%20Object%5D&name=image.png&originHeight=199&originWidth=581&originalType=binary&ratio=1&rotation=0&showTitle=false&size=39872&status=done&style=shadow&taskId=u6da8c10f-682f-4c2b-a8c4-3960c27fb13&title=&width=352.12119176915536)这样写数组的引用只可以传入大小为10的数组
<a name="MHR2D"></a>
#### 练习
<a name="qqdQP"></a>
##### 6.21
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658305630591-b50ebd9d-90ca-4ed5-814a-9e36180bab36.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=194&id=ud379f04a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1200&originWidth=1914&originalType=binary&ratio=1&rotation=0&showTitle=false&size=86186&status=done&style=shadow&taskId=ue89f83db-5366-4b7e-9d12-ce0d3f44f63&title=&width=309.9886169433594)<br />a写不写const都不会更改实参；<br />而b有可能传入的是数组
<a name="RzeS0"></a>
##### 6.22
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658305716784-00052866-4343-4914-8430-0f033fbfb9b0.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=154&id=ucee35b06&margin=%5Bobject%20Object%5D&name=image.png&originHeight=254&originWidth=725&originalType=binary&ratio=1&rotation=0&showTitle=false&size=64263&status=done&style=shadow&taskId=uc33a9827-a9fb-48d4-872e-1cfa97a0bb7&title=&width=439.3939139976551)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658305731777-d8894821-8840-42d3-9ab4-2827d410bfce.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=152&id=u4458e91a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=250&originWidth=782&originalType=binary&ratio=1&rotation=0&showTitle=false&size=71140&status=done&style=shadow&taskId=uf93c1656-5abe-45be-9f7f-df0c959f5c5&title=&width=473.9393665464363)<br />即使传入指针，实参内存地址也不会改变，除非使用二级指针或指针的引用↑
<a name="GqUJX"></a>
##### 6.24
输出数组ia前十个元素，可能导致越界，因为形参中的数组大小不起作用，ia如果只有5个元素还是可以传进函数，但会越界
<a name="x9src"></a>
### main：处理命令行选项
```cpp
int main(){...}
int main(int argc, char *argv[]){...}
```
程序处理的参数从argv[1]开始，argv[0]是可执行文件的名字
<a name="dFZAb"></a>
#### 练习
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658306140328-ec762c66-8941-420f-b3c3-664c9cb46323.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=418&id=u0e676846&margin=%5Bobject%20Object%5D&name=image.png&originHeight=662&originWidth=1185&originalType=url&ratio=1&rotation=0&showTitle=true&size=83229&status=done&style=shadow&taskId=uffd25248-a452-4394-a33c-2ef26089c02&title=Clion%E7%BB%99main%E4%BC%A0%E5%8F%82%E6%95%B0%E7%9A%84%E8%AE%BE%E7%BD%AE%E7%95%8C%E9%9D%A2&width=747.973388671875 "Clion给main传参数的设置界面")
<a name="paAoG"></a>
##### 6.25
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658306545372-75c26b91-6b5d-4d10-b134-8ebf98a38f86.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=176&id=u348ea837&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1050&originWidth=2142&originalType=binary&ratio=1&rotation=0&showTitle=false&size=77253&status=done&style=shadow&taskId=u9cf55968-c554-4a48-a293-13a03451b29&title=&width=358.973388671875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658306565907-2d77b145-3452-4360-8758-f2a0c5bbc47d.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=74&id=u1ab188de&margin=%5Bobject%20Object%5D&name=image.png&originHeight=122&originWidth=1279&originalType=binary&ratio=1&rotation=0&showTitle=false&size=16735&status=done&style=shadow&taskId=ua7874ada-cdfe-4ee7-bbbd-b0d1ae69172&title=&width=775.1514703489668)
<a name="NFami"></a>
### 含有可变形参的函数

- 实参类型相同，传递**initializer_list**类型
- 实参类型不同，写可变函数模板
- 省略符形参主要用于和C的接口

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658306821843-52b195c9-3b53-4191-beb4-e231aedf3315.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=367&id=uaec1b679&margin=%5Bobject%20Object%5D&name=image.png&originHeight=551&originWidth=1217&originalType=binary&ratio=1&rotation=0&showTitle=false&size=364963&status=done&style=shadow&taskId=u30a16bdc-38dd-46d4-95c6-d64d0edcc2d&title=&width=811.3333333333334)<br />初始化列表也是模板类型，类似vector；<br />list中的元素是常量，只可读不可写
<a name="yTH0c"></a>
#### 练习
<a name="KmFfj"></a>
##### 6.27
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658307389204-e923e173-4bb6-4970-82f5-d2a6268ac5b0.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=254&id=uaf454e37&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1500&originWidth=2352&originalType=binary&ratio=1&rotation=0&showTitle=false&size=119879&status=done&style=shadow&taskId=u25ea7ed9-f257-4c55-aed0-7ccce1108d9&title=&width=397.666748046875)
<a name="tKoqP"></a>
##### 6.28
其实elem不带const的话，auto推断出来也会是const string&类型，因为列表元素都是常量
<a name="Oeut7"></a>
## 6.3 返回类型和return语句

- 不要返回临时对象的指针或引用

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658307807280-91200d49-e91d-4c48-a3a0-7386cc3cfd09.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=247&id=uf7ca76f1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1200&originWidth=2160&originalType=binary&ratio=1&rotation=0&showTitle=false&size=111637&status=done&style=shadow&taskId=u323fd1e8-5b85-416f-9b08-99f86a9d41f&title=&width=444.666748046875)<br />返回临时对象或变量是可以的，但会导致拷贝开销，尽管有时不可避免

- return引用则返回左值，否则返回右值
<a name="dFQgR"></a>
#### 练习
<a name="OoRSD"></a>
##### 6.30
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658308305403-9957c8c5-d42d-4ee6-9fa9-499c275e21ce.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=263&id=uc2d215d0&margin=%5Bobject%20Object%5D&name=image.png&originHeight=394&originWidth=1981&originalType=binary&ratio=1&rotation=0&showTitle=false&size=92424&status=done&style=shadow&taskId=ub46f8e02-f3fe-4ad0-82b8-a4ef37129d1&title=&width=1320.6666666666667)<br />最下面的是本题的报错：return语句没有值（应该为bool）；for循环可能执行完，此时不写return会返回垃圾值（见习题6.6）
<a name="GtrXZ"></a>
### 返回数组指针
主要有三种写法：

1. type ( *function(p-list) ) [dimension]

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658318370143-815b20cc-1907-4f21-b5d4-0f47bc6b211d.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=187&id=u029b2d4b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=280&originWidth=1203&originalType=binary&ratio=1&rotation=0&showTitle=false&size=167875&status=done&style=shadow&taskId=ud7641c63-2284-4a47-b892-03865b02dc9&title=&width=802)<br />       ![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658318376993-ce65d07a-e9dd-4ce5-ad6f-d9e3d85d1e7e.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=38&id=ucd78d873&margin=%5Bobject%20Object%5D&name=image.png&originHeight=57&originWidth=956&originalType=binary&ratio=1&rotation=0&showTitle=false&size=29265&status=done&style=shadow&taskId=ud51282bd-654a-465d-a93d-f5b0568b76d&title=&width=637.3333333333334)<br />比较好理解的一种改善是数组使用别名，如typedef int arr[10]将arr声明为int [10]

2. **尾置返回类型**<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658319075304-06996d6b-9daf-4df8-b00e-dcfec364897f.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=59&id=u5cc0df86&margin=%5Bobject%20Object%5D&name=image.png&originHeight=89&originWidth=1129&originalType=binary&ratio=1&rotation=0&showTitle=false&size=53909&status=done&style=shadow&taskId=u5ba97c07-a1af-49f1-9f64-adcd66c1343&title=&width=752.6666666666666)<br />一般用于返回类型比较复杂的函数
3. decltype（数组名） *<br />要注意decltype不会把数组名当指针
<a name="X2zWs"></a>
#### 练习
<a name="YbHlk"></a>
##### 6.36 & 6.37
```cpp
string (& fun()) [10];//6.36

using string[10] = str_array;//最好的别名
//或者typedef string str_array[10]——太反人类
str_array & fun();//别名返回数组引用

auto fun() -> string(&)[10];//尾置类型返回数组引用
//还是尾置比较好理解

string arr[10];
decltype(arr)& fun();
```
<a name="yAjkA"></a>
## 6.4 函数重载

- 重载时形参的顶层const不区分<br />fun(int)和fun(const int)被视为相同的参数列表
- 区分底层const，涉及到类型转换<br />非const实参会优先选择非const形参进行匹配<br />此时可以用到const_cast
<a name="EoBHP"></a>
## 6.5 特殊语言特性
<a name="loxWH"></a>
### 默认实参

- 一个作用域中同一个函数一个形参只能拥有一个默认值

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658327516956-6a176b1c-acc6-4651-9339-6aa3601f7582.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=219&id=u40aca7f4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=328&originWidth=1223&originalType=binary&ratio=1&rotation=0&showTitle=false&size=153012&status=done&style=shadow&taskId=u152ff725-dace-4f63-a94b-59eb3214b94&title=&width=815.3333333333334)

- 局部变量不可以作默认参数
<a name="Pv1xn"></a>
#### 练习
<a name="ZrxYp"></a>
##### 6.42
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658328222156-86df3705-1553-40b4-8b21-65892046873b.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=291&id=u414aecd4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1650&originWidth=5316&originalType=binary&ratio=1&rotation=0&showTitle=false&size=347410&status=done&style=shadow&taskId=ubaf088fa-306f-407b-b19c-b471af6d36c&title=&width=937.666748046875)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658328260978-a6c3e237-553e-472f-a12e-2fa4d1feda21.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=98&id=ub2aac2b8&margin=%5Bobject%20Object%5D&name=image.png&originHeight=147&originWidth=443&originalType=binary&ratio=1&rotation=0&showTitle=false&size=17494&status=done&style=shadow&taskId=u50385240-f0f8-42a8-945f-0859ecceb77&title=&width=295.3333333333333)
<a name="zlJmW"></a>
### 内联函数和constexpr函数
这两类函数定义必须一致，经常实现在头文件

- 内联可省去函数开销（包括保存寄存器、参数拷贝、语句跳转）
- 内联只是请求，实现情况还是要看编译器

---

constexpr函数：

- 返回值和形参必须是字面值
- 有且仅有一条return
- 隐式指定为inline
- constexpr不一定返回常量表达式

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658328834949-1bb6d9dc-7516-430b-b94e-8b2e49cde075.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=295&id=KxLoG&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1500&originWidth=2208&originalType=binary&ratio=1&rotation=0&showTitle=false&size=129558&status=done&style=shadow&taskId=ue0ac73f4-889c-40a9-8527-d68c2daf44a&title=&width=434.66668701171875)尽管有红线，编译器并没有报错

---

<a name="d0sRZ"></a>
#### 字面值类型！
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658470936999-43b0eee9-cc42-4bf4-a451-b1fa670ca2f3.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=505&id=ud00f1abc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=757&originWidth=1767&originalType=binary&ratio=1&rotation=0&showTitle=false&size=118569&status=done&style=shadow&taskId=uced5855a-a246-4c39-8e37-a8189368a57&title=&width=1178)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658471029857-d38baba9-56d9-4be6-bc4c-e25942c35aaf.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=293&id=ua0eed7d7&margin=%5Bobject%20Object%5D&name=image.png&originHeight=439&originWidth=966&originalType=binary&ratio=1&rotation=0&showTitle=false&size=46808&status=done&style=shadow&taskId=u3e361b78-7560-4a39-803a-b56fb6fb5db&title=&width=644)<br />算术类型、枚举、指针、成员指针以及这些类型的const、volatile类型都算是标量/scalar type
<a name="IpR4v"></a>
### 调试帮助
assert()预处理宏；<br />NDEBUG预处理变量
<a name="KRHZ0"></a>
## 6.6 函数匹配
<a name="Y8Ucm"></a>
### 参数类型转换
<a name="Lm2m2"></a>
### ![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658329274333-895a34f0-20af-4a56-b14a-cb03b5f9e422.png#clientId=ue02841fc-6b51-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=446&id=u7db401f6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=669&originWidth=1281&originalType=binary&ratio=1&rotation=0&showTitle=false&size=380675&status=done&style=shadow&taskId=udaaa0fe7-5e54-4dc1-aac3-c1fbda1ddf3&title=&width=854)
第二点指非const指针或引用转换成const指针和引用（加上底层const）
<a name="RGYIE"></a>
#### 练习
<a name="MWuBM"></a>
##### 6.52
(a)两个char转int，属于第3级<br />(b)两个double转int，属于第4级
<a name="kN38K"></a>
##### 6.53
(c)会重复声明，重载不区分形参的顶层const
<a name="Icmp6"></a>
## 6.7 函数指针
用指针替换函数名即可，类似于指向数组的指针，函数名也被当作指针处理；<br />typedef函数指针和数组别名一样，比较反人类；<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658330051552-2a73a60e-0530-4655-8659-a63887eebbe2.png#clientId=uc59a2a1b-7d6d-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=64&id=u78ebed68&margin=%5Bobject%20Object%5D&name=image.png&originHeight=96&originWidth=991&originalType=binary&ratio=1&rotation=0&showTitle=false&size=44331&status=done&style=shadow&taskId=u8a3fe8b4-7555-4e65-ae59-625061f2319&title=&width=660.6666666666666)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658330058491-2a4ad6a9-1c11-4ae3-b61e-0fc940427a33.png#clientId=uc59a2a1b-7d6d-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=85&id=u6ecd5c01&margin=%5Bobject%20Object%5D&name=image.png&originHeight=127&originWidth=1130&originalType=binary&ratio=1&rotation=0&showTitle=false&size=88288&status=done&style=shadow&taskId=u10c47752-c144-4372-a5be-8211eb88c33&title=&width=753.3333333333334)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658330064128-81820699-2649-47cd-bcc5-6edccb13e294.png#clientId=uc59a2a1b-7d6d-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=31&id=u8ff068c5&margin=%5Bobject%20Object%5D&name=image.png&originHeight=46&originWidth=556&originalType=binary&ratio=1&rotation=0&showTitle=false&size=11348&status=done&style=shadow&taskId=u832cc22d-dc9d-4988-b717-623404348d2&title=&width=370.6666666666667)<br />decltype(函数名)也返回函数类型，需要加上*才是函数指针
<a name="Xakcp"></a>
#### 练习
<a name="GilqZ"></a>
##### 6.54
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658330276158-f1c0ba0b-0222-4e5f-a46d-c9b0fc3622a6.png#clientId=uc59a2a1b-7d6d-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=123&id=u46c9da74&margin=%5Bobject%20Object%5D&name=image.png&originHeight=450&originWidth=1794&originalType=binary&ratio=1&rotation=0&showTitle=false&size=52049&status=done&style=shadow&taskId=u1ca40295-6f04-4eb6-84d7-99be0ba1563&title=&width=490)
<a name="Cu5ED"></a>
##### 6.55 & 6.56
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658330592299-808fc0e2-22c1-4f35-afb4-34a613491ef8.png#clientId=uc59a2a1b-7d6d-4&crop=0&crop=0&crop=1&crop=0.5759&from=paste&height=798&id=ua671b00a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=4500&originWidth=2838&originalType=binary&ratio=1&rotation=0&showTitle=false&size=357721&status=done&style=shadow&taskId=u1cc47d68-0d39-4776-954d-f44178899f3&title=&width=503)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658330627799-975422fe-10dc-4775-87bf-84ee0775af14.png#clientId=uc59a2a1b-7d6d-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=383&id=ud5b5fce0&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1800&originWidth=2838&originalType=binary&ratio=1&rotation=0&showTitle=false&size=230855&status=done&style=shadow&taskId=u97b07839-dc0c-48c9-9d81-520b3bd39f1&title=&width=603.6666870117188)
<a name="zjkMn"></a>
# 第7章 类
第2章提过类，13章讲对象的行为包括复制、移动、销毁等，14章讲运算符重载；<br />类的用户应该是调用类的程序员，而程序的使用者是屏幕前的人；
<a name="oiYRk"></a>
## 7.1定义抽象数据类型
<a name="xtDNi"></a>
### 设计Sales_data类
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658375329706-c7d10723-f806-4578-b739-43bc07d7c9b1.png#clientId=ufb35da2a-17eb-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=184&id=u6354357c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=276&originWidth=1328&originalType=binary&ratio=1&rotation=0&showTitle=false&size=221984&status=done&style=shadow&taskId=u0119f914-5935-4b7d-b827-3f24ec468c1&title=&width=885.3333333333334)

- 成员函数声明在内部<br />	若定义在外部需要加类作用域：：<br />	定义在内部为隐式inline<br />实际上是通过this指针隐式访问对象，this是个指针常量
- 函数声明（）后加const为常量成员函数<br />	实际是给this加上底层const，因为不允许显式定义this
- 常量对象、常引用、常指针只能调用const成员函数，因为不允许通过调用改变对象
<a name="atRuj"></a>
#### 练习
<a name="eokWv"></a>
##### 7.4 & 7.5
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658378057441-7641db13-6919-42cf-bb4f-37e2a61ba970.png#clientId=ufb35da2a-17eb-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=259&id=u2239293e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1200&originWidth=2838&originalType=binary&ratio=1&rotation=0&showTitle=false&size=184528&status=done&style=shadow&taskId=u962f792d-63c3-4d2d-b14c-d3ba1e969e2&title=&width=613.666748046875)<br />应该定义为const成员函数，因为这些函数对对象都是只读不写
<a name="s0nfF"></a>
### 定义类相关的非成员函数

- 用到类的非成员函数概念上属于类的接口，但实际不属于类本身；

一般定义到头文件

- IO类不支持拷贝，只可以使用引用<br />不加#include<iostream>，<<无法重载
<a name="Me17m"></a>
#### 练习
<a name="FyjYW"></a>
##### 7.9
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658379350538-b64b9c0e-3226-46ce-9412-30162d757e0b.png#clientId=ufb35da2a-17eb-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=346&id=uf5dc5dac&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1800&originWidth=3246&originalType=binary&ratio=1&rotation=0&showTitle=true&size=176247&status=done&style=shadow&taskId=ud41940b0-fa7b-4270-8ae5-ec8c8211b65&title=Person.cpp&width=624.6666870117188 "Person.cpp")
<a name="yIma1"></a>
### 构造函数
有一些情况编译器无法生成默认构造函数，如数据成员包含另一个没有默认构造函数的类对象；

- =default可以保留默认行为，如构造函数、析构函数等
<a name="s2lYc"></a>
#### 练习
<a name="OIUKE"></a>
##### 7.13
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658385465274-1db34dc4-6bbe-4161-a5fd-a10275fd33c2.png#clientId=ufb35da2a-17eb-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=361&id=u2f6f14dc&margin=%5Bobject%20Object%5D&name=image.png&originHeight=542&originWidth=740&originalType=binary&ratio=1&rotation=0&showTitle=false&size=124090&status=done&style=shadow&taskId=u69ca8cbc-78c4-45c4-a35a-2a838508f61&title=&width=493.3333333333333)
<a name="XDJqM"></a>
##### 7.15
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658385621684-fc5a1010-87b4-489b-9b9c-e334ea6e9935.png#clientId=ufb35da2a-17eb-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=143&id=uf3fbac59&margin=%5Bobject%20Object%5D&name=image.png&originHeight=750&originWidth=3366&originalType=binary&ratio=1&rotation=0&showTitle=false&size=116219&status=done&style=shadow&taskId=uff008b89-8b56-4475-9ef6-6c322afbd20&title=&width=642.666748046875)<br />最好参数写成const引用
<a name="F0Mxi"></a>
### 拷贝、赋值和析构
复制/拷贝构造函数调用场景：

1. 用同类对象初始化另一个对象
2. 形参是对象，函数传参时调用
3. 返回值为函数局部临时对象
<a name="z4c3n"></a>
## 7.2 访问控制与封装
class第一个访问符之前默认为private；<br />struct默认为public；<br />还有继承时的访问权限，除此之外没有不同
<a name="r8AY7"></a>
### 友元
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658387276377-5cd9ebb2-35d5-4b4f-a2cd-bd5ed0d2b7f0.png#clientId=ufb35da2a-17eb-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=110&id=u1a1a2a69&margin=%5Bobject%20Object%5D&name=image.png&originHeight=450&originWidth=3534&originalType=binary&ratio=1&rotation=0&showTitle=false&size=106817&status=done&style=shadow&taskId=u39587da6-a11e-4c96-85a9-22a18b01a64&title=&width=866.666748046875)<br />函数是类接口的一部分但不是成员函数，且需要访问私有成员时，可以写为友元函数
<a name="I2Mrt"></a>
## 7.3 类的其他特性
<a name="lyDjq"></a>
### 可变数据成员
可变数据成员一直可以改变，即使是const对象、const成员函数；<br />指明数据成员为mutable<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658410744481-1695c357-a066-478b-b6fe-8b58c43b186c.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=379&id=uf78e105e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=568&originWidth=1366&originalType=binary&ratio=1&rotation=0&showTitle=true&size=213649&status=done&style=shadow&taskId=ue5397a6c-836f-4687-a942-ab566276833&title=mutable%E5%85%B3%E9%94%AE%E5%AD%97%E7%A4%BA%E4%BE%8B&width=910.6666666666666 "mutable关键字示例")
<a name="ecbX1"></a>
### 返回*this的成员函数

- const成员函数如果返回引用，则*this是const引用，不可以改变对象
- const成员函数谁都可以用，但非const成员函数只有非const对象才可以用<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658411503501-68d8f401-07b2-4013-9cab-4d4e6d77ece8.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=125&id=uc749a8da&margin=%5Bobject%20Object%5D&name=image.png&originHeight=187&originWidth=1023&originalType=binary&ratio=1&rotation=0&showTitle=false&size=107348&status=done&style=shadow&taskId=uae63f850-8939-41bc-bc7b-b3de4116aae&title=&width=682)
<a name="tE7hx"></a>
### 前向声明
在创建对象之前必须有类的定义；但类的名字出现之后就被认为声明过；<br />类的成员类型不可以是自己，但可以是同类的指针或引用<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658412453618-7c8ed41e-2a03-4b16-81bd-a97c2bbb1845.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=117&id=ufbe840ae&margin=%5Bobject%20Object%5D&name=image.png&originHeight=176&originWidth=662&originalType=binary&ratio=1&rotation=0&showTitle=false&size=14446&status=done&style=shadow&taskId=u8d8fdd13-0a05-40c3-84f9-66fea335c65&title=&width=441.3333333333333)因为不知道类的成员，所以这个类不完整
<a name="kbXUZ"></a>
#### 练习
<a name="tkC3w"></a>
##### 7.31
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658412551332-112b3378-8d7b-4ef6-9780-ce2a7e64879e.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=251&id=u1d1420bb&margin=%5Bobject%20Object%5D&name=image.png&originHeight=376&originWidth=209&originalType=binary&ratio=1&rotation=0&showTitle=false&size=13509&status=done&style=shadow&taskId=ub7b89713-65ab-4fa3-8154-efa6c6779d0&title=&width=139.33333333333334)必须有Y的前向声明，否则会报错![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658412592926-e586244f-50e1-4c4e-a43a-710a4e89f344.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=120&id=u68616fb1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=180&originWidth=327&originalType=binary&ratio=1&rotation=0&showTitle=false&size=9658&status=done&style=shadow&taskId=u2bfb6e26-22a1-42cc-803e-bb3b60ab4ce&title=&width=218)
<a name="UbEBe"></a>
### 友元类
除了非成员函数定义为友元还有两种友元：

1. 声明友元类<br />友元类的成员函数可以访问此类的所有成员<br />友元类无传递性
2. 声明已定义类的成员函数<br />加上类作用域，当然这个类需要定义过<br />重载的函数需要一一声明

**友元声明和作用域**——易错<br />友元函数最好是类内声明，类外定义；<br />即使是类内定义，类外也需要写一次，否则作用域只限于类内，外部不可见<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658413552712-79dd5b70-a2f1-4e4c-8c6c-c44cba2881d4.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=189&id=u2c4cc05b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=284&originWidth=327&originalType=binary&ratio=1&rotation=0&showTitle=true&size=13626&status=done&style=shadow&taskId=uf04d74d8-6dea-4de3-9f0d-8a0f952b954&title=%E6%AD%A3%E7%A1%AE%E5%86%99%E6%B3%95%EF%BC%8Cf%28%29%E5%A3%B0%E6%98%8E%E5%9C%A8%E5%89%8D%E9%9D%A2&width=218 "正确写法，f()声明在前面")<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658414447203-209a58d5-6c73-4a9f-b202-c3356cce6337.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=189&id=ucbd5280a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=283&originWidth=345&originalType=binary&ratio=1&rotation=0&showTitle=false&size=13667&status=done&style=shadow&taskId=u0d91dac8-165b-417f-b034-44bae6fcc17&title=&width=230)虽然友元函数实现了，但是构造函数中仍不可见，因为f声明在类后<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658414792528-8eac5490-75f0-4d2f-883a-14999b100311.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=171&id=u44a04f7d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1050&originWidth=1332&originalType=binary&ratio=1&rotation=0&showTitle=false&size=48204&status=done&style=shadow&taskId=uaa04bb54-ebf2-4d72-9af5-f516ac7c384&title=&width=217)即使实现在类内也一样对于其他函数不可见
<a name="HLyNd"></a>
## 7.4 类的作用域
<a name="spuPa"></a>
### 名字查找和类的作用域
名字查找分三步：

1. 当前块这一句之前找声明
2. 找外层
3. 没找到就报错

---

类定义分两步：

1. 编译成员的声明
2. 类全部可见后编译**成员函数**体

除成员函数外使用的名字都必须确保声明过<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658415164399-01815915-3364-4fed-a4e2-a88d90f30dee.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=141&id=ue93dbdc6&margin=%5Bobject%20Object%5D&name=image.png&originHeight=211&originWidth=521&originalType=binary&ratio=1&rotation=0&showTitle=false&size=40533&status=done&style=shadow&taskId=ue85a614d-3edd-414e-80d9-7d5170acd4b&title=&width=347.3333333333333)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658415169403-1c976c59-416d-47cf-9481-c4843b0291c6.png#clientId=u74fd8e93-cbee-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=170&id=u383e5fb3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=255&originWidth=810&originalType=binary&ratio=1&rotation=0&showTitle=false&size=40921&status=done&style=shadow&taskId=u0a824f67-93d5-4448-9484-51573b9d978&title=&width=540)<br />类内Money自然是double类型，而bal从类内先找声明，因此是double类型而非全局变量string类型<br />成员函数解析过程：

1. 函数内
2. 类内所有成员
3. 类外部函数定义之前的全局作用域
<a name="qgzKw"></a>
#### 练习
<a name="RFNcS"></a>
##### 7.34
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658459918816-9b146523-f6c5-451a-813b-24e2a70025ed.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=329&id=u031a8a1a&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1500&originWidth=2436&originalType=binary&ratio=1&rotation=0&showTitle=false&size=131761&status=done&style=shadow&taskId=uf6f2f9c1-1c45-4985-ace6-9e68ba9be35&title=&width=533.6666870117188)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460068250-8249df24-b51d-4465-bdba-9cfa794bda46.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=131&id=u837c48e9&margin=%5Bobject%20Object%5D&name=image.png&originHeight=196&originWidth=1306&originalType=binary&ratio=1&rotation=0&showTitle=false&size=39465&status=done&style=shadow&taskId=u4b612f33-7aca-461a-a3b1-cb109b04469&title=&width=870.6666666666666)
<a name="Lm9p8"></a>
##### 7.35
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460533149-106874bb-7692-4c00-b762-66bee61ea4ae.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=396&id=ue47a9864&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2400&originWidth=4092&originalType=binary&ratio=1&rotation=0&showTitle=false&size=215776&status=done&style=shadow&taskId=ued9aafee-8077-4d01-83e3-3909f874c3e&title=&width=674.6666870117188)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460557942-86e6ffc1-16d4-45a4-9931-673607d31e74.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=69&id=u4705093d&margin=%5Bobject%20Object%5D&name=image.png&originHeight=103&originWidth=1774&originalType=binary&ratio=1&rotation=0&showTitle=false&size=27706&status=done&style=shadow&taskId=u534ae3b8-3302-4c2e-933f-7ce3d22f14a&title=&width=1182.6666666666667)
<a name="mAo20"></a>
## 7.5 构造函数
<a name="rLbL4"></a>
### 初始值列表

- 第一种普通情况

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460732228-127b933e-7515-4def-b3ef-1195b7c9593e.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=64&id=ua6fc94c3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=96&originWidth=1182&originalType=binary&ratio=1&rotation=0&showTitle=true&size=70399&status=done&style=shadow&taskId=u089f84e5-9b15-4bff-8332-68edd09a95c&title=%E5%88%97%E8%A1%A8%E5%88%9D%E5%A7%8B%E5%8C%96&width=788 "列表初始化")<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460759651-f4400b74-0b55-4c16-815c-9190976c80c4.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=214&id=u3574e8f3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=321&originWidth=1021&originalType=binary&ratio=1&rotation=0&showTitle=true&size=86951&status=done&style=shadow&taskId=ub3cc3840-e55a-41d4-b011-776c8f1b7f8&title=%E7%AC%AC%E4%BA%8C%E7%A7%8D%E5%86%99%E6%B3%95&width=680.6666666666666 "第二种写法")<br />此时两者效果相同，但是初始化和赋值操作还是有差别，完全取决于成员类型，初始化一定是比赋值开销小的

---

- 第二种成员含const、引用和无默认构造函数的类对象

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460855943-0e28e3d1-3a15-489d-8c03-d269307c8f9d.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=252&id=uc08822b8&margin=%5Bobject%20Object%5D&name=image.png&originHeight=378&originWidth=457&originalType=binary&ratio=1&rotation=0&showTitle=false&size=62065&status=done&style=shadow&taskId=ua2c5e576-d92c-4ded-ab2f-629060d95f6&title=&width=304.6666666666667)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658460862839-83cbb964-4df4-4c59-b452-e6f1c01c9c18.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=219&id=u4c96a04b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=329&originWidth=1056&originalType=binary&ratio=1&rotation=0&showTitle=false&size=107844&status=done&style=shadow&taskId=u196f9560-2287-4fdf-aec5-cf4efc8380b&title=&width=704)<br />由于const和引用必须初始化，不允许声明后再赋值，所以必须要用初始值列表；<br />没有默认构造函数的类对象被当作成员时需要初始化，否则无法构造对象成员<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463010276-056ed4f3-171e-45f6-831c-8e5d669d0d40.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=320&id=ucd84f7a3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=1800&originWidth=1332&originalType=binary&ratio=1&rotation=0&showTitle=false&size=81416&status=done&style=shadow&taskId=ub4b12430-3890-4972-bda6-d87645fea8b&title=&width=237)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463086649-1258398a-6aad-4502-b44f-21a663a8bc15.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=247&id=u2eb04f27&margin=%5Bobject%20Object%5D&name=image.png&originHeight=371&originWidth=1479&originalType=binary&ratio=1&rotation=0&showTitle=false&size=94732&status=done&style=shadow&taskId=ub33d110d-0ca9-46cd-89a1-bd144004564&title=&width=986)<br />B的构造函数是默认的，没有显式构造对象a<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463313828-00a6ec94-0db7-4d71-9772-53d007edae10.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=437&id=u193ed20c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=2100&originWidth=1446&originalType=binary&ratio=1&rotation=0&showTitle=false&size=116882&status=done&style=shadow&taskId=ud046ceba-d0ac-4954-9155-c41beeb4c34&title=&width=301)B构造函数需要构造自己的对象成员，尤其是那个成员没有默认构造函数时
<a name="IzvhL"></a>
### 成员初始化顺序
初始值列表只说明值，不指示初始化顺序；一般依据成员定义出现的顺序进行初始化；<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463500621-81157158-4bcd-4eb2-a9a2-1ae1fd1b838a.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=226&id=u0d18701b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=339&originWidth=704&originalType=binary&ratio=1&rotation=0&showTitle=false&size=66516&status=done&style=shadow&taskId=ube3d82de-23b3-44fd-a569-e673c362116&title=&width=469.3333333333333)<br />i先声明，所以尽管列表中j写在前面，还是先初始化i，但是j的值未定义，可能会报错；<br />因此尽量避免用一个成员初始化另一个成员；

---

当构造函数所有参数都有默认值时，相当于提供了默认构造函数
<a name="XjKSs"></a>
#### 练习
<a name="YAS2Q"></a>
##### 7.36
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463733780-b3b60f10-61a0-4121-87f9-4b18e3298245.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=128&id=u503ebbbe&margin=%5Bobject%20Object%5D&name=image.png&originHeight=192&originWidth=993&originalType=binary&ratio=1&rotation=0&showTitle=false&size=22175&status=done&style=shadow&taskId=u664baf47-c23e-4ca5-97d4-71a2e5c460d&title=&width=662)<br />和上面提到的例子相同，用了未定义的base初始化rem；<br />自定义类还是注意下顺序
<a name="VSGti"></a>
##### 7.37
本节定义参考如下<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463811615-06bc105c-b56d-41c2-bd3e-3502e77b487a.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=311&id=ub0f39008&margin=%5Bobject%20Object%5D&name=image.png&originHeight=467&originWidth=1300&originalType=binary&ratio=1&rotation=0&showTitle=false&size=253806&status=done&style=shadow&taskId=u2a717f0a-df32-4e27-ad6f-7e15bc77553&title=&width=866.6666666666666)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658463857027-301c36b7-9f1e-4b6b-a2ad-a2a764b2c304.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=82&id=u2cc48d53&margin=%5Bobject%20Object%5D&name=image.png&originHeight=123&originWidth=376&originalType=binary&ratio=1&rotation=0&showTitle=false&size=13542&status=done&style=shadow&taskId=u7e412be9-70f4-4b0c-82e6-8255b7858c3&title=&width=250.66666666666666)<br />next默认初始化，bookNo为空串，其他为0；<br />last的bookNo为9-999-99999-9，其他为0；<br />两者都是用第一个构造函数
<a name="XWSTR"></a>
##### 7.38
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658466189206-a1950746-3606-47e7-b3cb-22ca415318c0.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=156&id=uc8a9911f&margin=%5Bobject%20Object%5D&name=image.png&originHeight=750&originWidth=2142&originalType=binary&ratio=1&rotation=0&showTitle=false&size=43834&status=done&style=shadow&taskId=uc55517cb-ea9b-4621-8065-c7f66fe8c23&title=&width=446.666748046875)
<a name="f7PE1"></a>
### 委托构造函数！
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658466505482-9a8319a6-9f57-47d5-8648-7f174b544c0e.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=128&id=ud3a9293f&margin=%5Bobject%20Object%5D&name=image.png&originHeight=192&originWidth=1231&originalType=binary&ratio=1&rotation=0&showTitle=false&size=129504&status=done&style=shadow&taskId=uba968136-c07d-4896-a16e-98d95943e1b&title=&width=820.6666666666666)<br />A委托B帮他构造，先执行B代码，然后返还A继续执行
<a name="drOtg"></a>
### 默认构造函数
内置类型和复合类型的成员只有在对象是全局作用域时才初始化，否则是垃圾值<br />默认初始化发生在：

- 局部作用域定义非静态对象或数组
- 类的成员有对象且使用默认构造函数
- 类的对象成员没有在初始值列表中显式初始化

值初始化发生在：

- 数组初始化列表中元素不够
- 局部静态变量
- classname a()使用只含一个参数的构造函数请求值初始化
<a name="L8e19"></a>
### 隐式的类类型转换
如果构造函数只有一个参数，又叫转换构造函数，实际上定义了其他类型转换为此类的隐式规则；<br />explicit加在声明前可以阻止隐式转换，不过只能写在**类内声明**前，定义的时候不要再重复explicit；<br />explicit只能用于直接初始化，拷贝初始化/=都不行；<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1659779764897-fd0d306d-5789-48de-8f77-b7bc2ad540e7.png#clientId=ue407e082-2104-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=497&id=u1e9f175b&margin=%5Bobject%20Object%5D&name=image.png&originHeight=820&originWidth=770&originalType=binary&ratio=1&rotation=0&showTitle=false&size=64914&status=done&style=shadow&taskId=u8641a8e7-d6d1-44e5-89e0-1d5e9388dc1&title=&width=466.6666396940613)<br />编译器只会执行一步隐式类类型转换<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658468185995-bc64c33c-13cb-45a5-9993-bd926371c9e1.png#clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=131&id=u6b7eee20&margin=%5Bobject%20Object%5D&name=image.png&originHeight=196&originWidth=916&originalType=binary&ratio=1&rotation=0&showTitle=false&size=109953&status=done&style=shadow&taskId=u5af38b9c-5c4e-4dfe-b2c9-868d7d2edea&title=&width=610.6666666666666)

- string接收const string*的构造函数不是explicit<br />所以可以=初始化
- vector接收容量的构造函数是explicit

![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658468023622-3c66bbd9-261b-4e42-8424-4ab2535ccfcb.png#averageHue=%23fdfdfc&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=266&id=u8e229cdb&margin=%5Bobject%20Object%5D&name=image.png&originHeight=399&originWidth=998&originalType=binary&ratio=1&rotation=0&showTitle=false&size=37773&status=done&style=shadow&taskId=uf39279df-7254-4fd0-8649-c269f1b8a94&title=&width=665.3333333333334)
<a name="xMKQd"></a>
#### 练习
<a name="IXvTh"></a>
##### 7.49
![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658469115358-108d6fdf-50c4-4b5a-96ba-fac955d4967e.png#averageHue=%23fcfbfa&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=278&id=u591c44f3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=417&originWidth=444&originalType=binary&ratio=1&rotation=0&showTitle=false&size=28600&status=done&style=shadow&taskId=u7c379a28-583f-41fa-a147-621e1ca3ca5&title=&width=296)<br />注意非const引用不可以绑定临时对象！

- 以引用的方式传递一个临时变量做为函数参数，如果函数内部对此临时变量做了修改，那么函数返回后，程序员无法获得函数对临时变量的修改。函数对临时变量所做出的所有更改，都将丢失
- C++中产生的临时对象是不可修改的<br />默认为const的非常量引用必须绑定左值，**非const引用只能绑定到与该引用同类型的对象，而const引用则可以绑定到不同的但相关的对象或绑定到右值**<br />非const不可以转换为const类型
- C++标准的规定：非常量的引用不能指向临时对象
<a name="vOutA"></a>
##### 7.51
vector<int> v=1;<br />这种写法不清楚是初始化容量还是元素值，禁止这种二义性，（所以我猜）v的单参构造函数是explicit<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658469772357-110c50e5-7064-45d7-a494-c6da2460dcb2.png#averageHue=%23ececec&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=162&id=u10535c52&margin=%5Bobject%20Object%5D&name=image.png&originHeight=243&originWidth=1541&originalType=binary&ratio=1&rotation=0&showTitle=false&size=245295&status=done&style=shadow&taskId=ubdf9b1c5-8f4a-4df1-88e5-5ca7d0cafc3&title=&width=1027.3333333333333)
<a name="infFY"></a>
### 聚合类

- 全public
- 无构造函数
- 没有类内成员初始值
- 没有基类、没有virtual函数

这样的类可以用初始值列表初始化<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658469866171-0ab1e22c-8da5-4377-9436-11517972b374.png#averageHue=%23f5f5f5&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=129&id=uad3a66d1&margin=%5Bobject%20Object%5D&name=image.png&originHeight=193&originWidth=358&originalType=binary&ratio=1&rotation=0&showTitle=false&size=25630&status=done&style=shadow&taskId=uf7c1a6ad-e696-40b2-89ff-47f60efdab2&title=&width=238.66666666666666)![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658469872386-880a809e-1f11-458c-bd32-c458888cbd0d.png#averageHue=%23f3f3f3&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=39&id=u6cb7c608&margin=%5Bobject%20Object%5D&name=image.png&originHeight=59&originWidth=592&originalType=binary&ratio=1&rotation=0&showTitle=false&size=16004&status=done&style=shadow&taskId=u9c5db4cc-b0de-4fe2-a5c4-d36f446015b&title=&width=394.6666666666667)<br />如果表里元素不够，剩下的被值初始化
<a name="o1o6T"></a>
### 字面值常量类
不知道有啥用，要求也很繁琐，暂时略过，看不到应用场景<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658486426949-aa1d1fc0-207e-4f93-9d1c-3264776a45a1.png#averageHue=%23efefef&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=344&id=uc1e8c5d2&margin=%5Bobject%20Object%5D&name=image.png&originHeight=516&originWidth=1520&originalType=binary&ratio=1&rotation=0&showTitle=false&size=425428&status=done&style=shadow&taskId=u1c4869a8-1de5-44e8-a24a-d3ac9059cb7&title=&width=1013.3333333333334)<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658486566092-dc6b86a4-43a6-4f28-bedc-2d6d99175a0f.png#averageHue=%23f4f2f1&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=277&id=uf0237728&margin=%5Bobject%20Object%5D&name=image.png&originHeight=415&originWidth=1367&originalType=binary&ratio=1&rotation=0&showTitle=false&size=134120&status=done&style=shadow&taskId=u65d194f2-0705-4090-afcb-49d3a646f93&title=&width=911.3333333333334)
<a name="R1B0a"></a>
## 7.6 类的静态成员

- 属于类不属于对象
- 不能为const，不能使用this
- static只出现在类内部的声明
- 必须在外部定义和初始化静态成员<br />为保证只定义一次，最好static和非内联函数的定义放一起
<a name="MBfrT"></a>
### 类内初始化
非常量静态成员不可以类内初始化<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658487325785-f9c63a60-cf92-4a81-9787-55aef67d2de3.png#averageHue=%23fafbe8&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=85&id=u278c8d96&margin=%5Bobject%20Object%5D&name=image.png&originHeight=127&originWidth=772&originalType=binary&ratio=1&rotation=0&showTitle=false&size=9580&status=done&style=shadow&taskId=u7c09c829-4862-4907-9282-b2ab513549c&title=&width=514.6666666666666)<br />如果是常量表达式则可以类内初始化<br />![image.png](https://cdn.nlark.com/yuque/0/2022/png/21578825/1658487376040-60245217-dac9-4ff3-a224-76cc85e705fa.png#averageHue=%23fefefd&clientId=ua8ff9e7e-e2e3-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=41&id=uc15629fb&margin=%5Bobject%20Object%5D&name=image.png&originHeight=62&originWidth=521&originalType=binary&ratio=1&rotation=0&showTitle=false&size=4982&status=done&style=shadow&taskId=udbd5e704-0f47-4c1c-b15b-a11147835ec&title=&width=347.3333333333333)<br />const还可以类内声明类外定义

---

静态数据成员可以是不完全类型（声明且没有完整定义）；<br />静态成员可以作默认实参；非静态成员属于对象，作参数不知道属于哪个对象会报错


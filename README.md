# ConstraintLayout

### 这个demo 的参考地址 https://developer.android.google.cn/reference/android/support/constraint/ConstraintLayout#VirtualHelpers  
### https://blog.csdn.net/lmj623565791/article/details/78011599?utm_source=tuicool&utm_medium=referral  
### 效果图  
![img](https://github.com/leon5458/ConstraintLayout/blob/master/ConstraintLayout/1.png)   

### 自己参考写了一个demo 顺便说下自己的思路,之前一直以为约束布局它是拖拽类型的每次都是直接删除掉了
### 这次自己把它理解为相对布局,但是不是说是,
###   android:layout_marginLeft="20dp" 这个相对左边在约束布局中写 app:layout_constraintLeft_toLeftOf="parent" 才会移动,自己的理解为约束布局的左边相对于父布局的左边,  
### 如果距离顶部, 就会用约束布局的顶部相对于父布局的顶部,这个才会达到移动  
### 相对于某个位置的在什么什么地方情况类似, 例如demo中tv1的顶部位于banner底部,tab1的左边位于tab2的右边,这个都是相对的,
### 自己按照这个理解约束布局就很简单了,写的时候可以写后面的,to+(R,L,B,T)这是个位置能更好的提示,然后就会有提示,   
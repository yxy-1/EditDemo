# EditDemo
只是测试demo，需要几个步骤，实现 Android EditText弹出软键盘实现页面标题头不动，软键盘弹出在编辑框下面

1.页面根布局使用相对布局-RelativeLayout，demo中使用的是activity_main.xml

2.EditText所在的布局中（可以是复杂的组合布局包含），必须位于根布局的底部，也就是写android:layout_alignParentBottom=”true”这个属性，即demo中的EditText控件

3.弹出软键盘时，需要一起被弹起的布局添加 android:layout_above="@+id/et_test" 也就是demo中的示例ImageView控件

4.配置文件里面该activity要设置android:windowSoftInputMode=”adjustResize”,即清单文件中MainActivity设置   

<activity android:name=".MainActivity"
          android:windowSoftInputMode="adjustResize">
          
语言不太容易描述，希望可以有所帮助，也是我自己的记录

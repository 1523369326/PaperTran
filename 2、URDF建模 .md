# 2、URDF建模

本章节介绍URDF建模机械臂，然后利用别人提供的机械臂模型在matlab做一下简单的操作然后到处成URDF格式，在ros中使用

### URDF建模原理

![Untitled](2%E3%80%81URDF%E5%BB%BA%E6%A8%A1%20640df042564d40b18983d45db8fdf072/Untitled.png)

![Untitled](2%E3%80%81URDF%E5%BB%BA%E6%A8%A1%20640df042564d40b18983d45db8fdf072/Untitled%201.png)

![Untitled](2%E3%80%81URDF%E5%BB%BA%E6%A8%A1%20640df042564d40b18983d45db8fdf072/Untitled%202.png)

### XACRO优化

但是URDF操作冗余，使用xacro模型文件优化，教程如下

![Untitled](2%E3%80%81URDF%E5%BB%BA%E6%A8%A1%20640df042564d40b18983d45db8fdf072/Untitled%203.png)

![Untitled](2%E3%80%81URDF%E5%BB%BA%E6%A8%A1%20640df042564d40b18983d45db8fdf072/Untitled%204.png)

![Untitled](2%E3%80%81URDF%E5%BB%BA%E6%A8%A1%20640df042564d40b18983d45db8fdf072/Untitled%205.png)

### 代码讲解

`material` 元素通常包含以下属性：

- `name`：材质的名称。
- `color`：材质的颜色，通常由四个浮点数表示，分别是红色、绿色、蓝色和透明度（alpha）值。
- `texture`：材质的纹理，通常是一个指向纹理文件的路径。

```cpp
<material name="Black">
        <color rgba="0 0 0 1"/>
</material>
```

这个元素定义了一个名为 "Black" 的材质，它的颜色是黑色，不透明。
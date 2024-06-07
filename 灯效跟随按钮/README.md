本例中实现原理与之前的流水灯边框几乎相同，都是使用伪元素负责发光，然后在使用伪元素进行遮罩
将多余的部分hidden掉，然后配合js，获取光标坐标，修改为元素的定位坐标
然后添加过渡，最终实现光效跟随效果

background: radial-gradient(var(--clr), transparent, transparent);  创建一个以原点为中心的向外辐射的光效
opacity: 1; 可以理解为透明度，或可是程度，0未不可视，1为完全不透明
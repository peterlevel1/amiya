# 商品编辑

<Badge>AyForm</Badge>

复杂程度：⭐️⭐️⭐️

遇到复杂的表单元素时，可把整个内容封装成一个组件，只要组件支持受控（提供 onChange、value）方法，就可以作为表单元素，如下面的`商品信息`部分。

表单并不自带上传组件，如果遇到，可参考代码自行封装。

卡片分组非常常见，也可以配合 `Anchor` 组件进行联动定位。

联动时注意多测试性能，如果你只想用户操作时触发更新，就不要通过 useEffect 去触发联动更新，转成自己手动触发 ，这是个大坑，且会在没有必要时触发更新。

<code src="./page/index.tsx" />
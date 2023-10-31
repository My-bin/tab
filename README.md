# tab切换
tab组件

用法

```vue
 <Tabs v-model="activeName" @tab-click="tabClick">
      <TabsPanel
        v-for="item in orderStatus"
        :label="item.label"
        :name="item.name"
      >
      </TabsPanel>
    </Tabs>
```

参数

activeName 激活项name  v-model绑定

label 展示数据

name 相当于（value）

tab-click点击某项的回调方法


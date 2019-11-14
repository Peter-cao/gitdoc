# dialog
交互

<h2 id="cid_2">示例</h2>

```html
//toast
agileBridge.dialog.toast("这是一条消息",()=>{
    
})

//显示loading
 agileBridge.dialog.showLoading();

//隐藏loading
agileBridge.dialog.hideLoading();

//alert
agileBridge.dialog.alert("这是一条消息",()=>{
    console.info("点击了确定")
});

//confirm
confirm: function(){
    agileBridge.dialog.confirm("确定删除吗",()=>{
        console.info("点击了确定")
    },()=>{
        console.info("点击了取消")
    });
},

//showActionSheet
agileBridge.dialog.showActionSheet({
    items: ['菜单一', '菜单二', '菜单三'],
    success:function(index){
        console.log(`点击了第${index}个`)
    },
    fail:function(e){
        console.log(e)
    }
});
```
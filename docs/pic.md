# pic
图片选择。
<h2 id="cid_2">参数</h2>
<table>
    <tr>
        <th>参数</th>
        <th>说明</th>
        <th>类型</th>
        <th>必填</th>
        <th>默认值</th>
    </tr>
    <tr>
        <td>success</td>
        <td>接口调用成功的回调函数</td>
        <td>function</td>
        <td>否</td>
        <td>-</td>
    </tr>
    <tr>
        <td>fail</td>
        <td>接口调用失败的回调函数</td>
        <td>function</td>
        <td>否</td>
        <td>-</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
agileBridge.pic.chooseImage({
    success:function(path,args){
        let imgSrc = self.data.imgSrc;
        imgSrc.push(path);
        self.setData({
            imgSrc:imgSrc
        })
        if(args){//网页chooseImage 回调函数中第二个参数为要上传的file本身
            self.file.push(args);
        }else{
            self.file.push(path);
        }
    },
    error:function(error){
        console.log(error)
    }
})
```
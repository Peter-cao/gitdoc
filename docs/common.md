
# 公共说明

这里主要介绍对于页面和组件以及使用上的一些说明。


<h2 id="cid_1">公共方法</h2>

页面和组件具有一些公共方法，方便进行一些简单操作。 

<table>
    <tr>
        <th>方法名</th>
        <th>说明</th>
        <th>参数</th>
        <th>返回值</th>
    </tr>
    <tr>
        <td>selectById</td>
        <td>根据id获取组件对象</td>
        <td>String id</td>
        <td>Component</td>
    </tr>
    <tr>
        <td>selectByName</td>
        <td>根据name获取组件对象</td>
        <td>String name</td>
        <td>[Component]</td>
    </tr>
    <tr>
        <td>selectBySelector</td>
        <td>根据选择器获取组件对象（仅支持id、class，浏览器下可支持全选择器）</td>
        <td>String selector</td>
        <td>[Component]</td>
    </tr>
    <tr>
        <td>getValueByName</td>
        <td>根据name获取组件的value（仅限单选、多选组件）</td>
        <td>String name</td>
        <td>any</td>
    </tr>
    <tr>
        <td>getValuesByName</td>
        <td>根据name获取组件的value（仅限多选组件）</td>
        <td>String name</td>
        <td>Array</td>
    </tr>
    <tr>
        <td>getAttrValue</td>
        <td>获取组件的属性值</td>
        <td>String propName（组件名）</td>
        <td>any</td>
    </tr>
    <tr>
        <td>setData</td>
        <td>设置数据，设置内部数据，并渲染至页面</td>
        <td>Object data</td>
        <td>void</td>
    </tr>
    <tr>
        <td>triggerEvent</td>
        <td>往组件外部触发事件</td>
        <td>String eventName（事件名）, Object detail（传递的参数）</td>
        <td>void</td>
    </tr>
    <tr>
        <td>getAbsolute</td>
        <td>文件绝对路径，一般在跨组件并且js动态设置图片路径时使用</td>
        <td>String path（文件路径）</td>
        <td>String</td>
    </tr>
</table>

<h2 id="cid_2">公共样式说明</h2>


1. 公共样式问题

由于微信小程序的组件是封闭，内部的css不会共享，而h5的样式是共享的。

如果确实有需要css共享的，可以新建一个文件名为<code>组件名.common.css</code>文件，这个文件会在所有页面中引入。

当然，也可以在任意地方建一个css文件，所有页面自行引入也可以。这样会节约开销。

2. 对于less、sass等的支持

目前暂不支持，但如果确定仅运行于浏览器，可以在style标签上设置type="less"


3. 关于布局

目前基本上的布局方式都以flex为主，对于移动端基本够用，故display基本只设置为flex， block、inline-block等不应该使用。


4. 长度单位使用

目前建议使用rem为统一长度单位，也可使用px，rem的相对像素为12px。


<h2 id="cid_3">jsapi问题</h2>

1. 由于jsapi封装了部分微信公众号的jssdk，而其需要进行微信授权方能使用，所以需要页面中调用wx.config进行配置

2. 小程序中调用部分jsapi需要在其IDE中设置权限，以及最终发布的时候也需要申请相关权限，请在具体的平台中进行操作



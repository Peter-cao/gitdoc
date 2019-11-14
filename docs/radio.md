# radio
单选项目。
<h2 id="cid_1">属性</h2>
<table>
    <tr>
        <th>属性</th>
        <th>说明</th>
        <th>类型</th>
        <th>可选值</th>
        <th>默认值</th>
    </tr>
    <tr>
        <td>value</td>
        <td>&lt;radio&gt;标识，选中时触发&lt;radio-group&gt;的 change 事件，并携带 &lt;radio&gt; 的 value</td>
        <td>String</td>
        <td>-</td>
        <td></td>
    </tr>
    <tr>
        <td>disabled</td>
        <td>是否禁用</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>checked</td>
        <td>当前是否选中，可用来设置默认选中</td>
        <td>Boolean</td>
        <td>-</td>
        <td>false</td>
    </tr>
    <tr>
        <td>color</td>
        <td>radio的颜色，同css的color</td>
        <td>String</td>
        <td>-</td>
        <td>#09bb07</td>
    </tr>
</table>

<h2 id="cid_2">事件</h2>

<table>
    <tr>
        <th>事件名</th>
        <th>说明</th>
        <th>参数</th>
    </tr>
    <tr>
        <td>click</td>
        <td>点击事件，切换checked状态</td>
        <td>-</td>
    </tr>
</table>

<h2 id="cid_2">示例</h2>

```html
 <view class="form-detail-item">
    <text>同步到：</text>
    <axi-label for="wx1">
        <axi-radio id="wx1" name="share" v-model:radio="formData.detail.share1" value="1"></axi-radio>
        <text class="pr6">微信</text>
    </axi-label>
    <axi-label for="dd1">
        <axi-radio id="dd1" name="share" v-model:radio="formData.detail.share1" value="2"></axi-radio>
        <text class="pr6">钉钉</text>
    </axi-label>
    <axi-label for="wb1">
        <axi-radio id="wb1" name="share" v-model:radio="formData.detail.share1" value="3"></axi-radio>
        <text>微博</text>
    </axi-label>
</view>
```
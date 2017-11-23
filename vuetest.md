{% raw %}
<div id="example-5">
  <select v-model="selected">
    <option disabled value="">请选择</option>
    <option>A</option>
    <option>B</option>
    <option>C</option>
  </select>
  <span>Selected: {{ selected }}</span>
</div>
<script>
new Vue({
  el: '#example-5',
  data: {
    selected: ''
  }
})
</script>
{% endraw %}

<p class="tip">如果 `v-model` 表达初始的值不匹配任何的选项，`<select>` 元素就会以"未选中"的状态渲染。在 iOS 中，这会使用户无法选择第一个选项，因为这样的情况下，iOS 不会引发 change 事件。因此，像以上提供 disabled 选项是建议的做法。</p>

多选列表 (绑定到一个数组)：

``` html
<div id="example-6">
  <select v-model="selected" multiple style="width: 50px;">
    <option>A</option>
    <option>B</option>
    <option>C</option>
  </select>
  <br>
  <span>Selected: {{ selected }}</span>
</div>
```

``` js
new Vue({
  el: '#example-6',
  data: {
    selected: []
  }
})
```

{% raw %}
<div id="example-6">
  <select v-model="selected" multiple style="width: 50px;">
    <option>A</option>
    <option>B</option>
    <option>C</option>
  </select>
  <br>
  <span>Selected: {{ selected }}</span>
</div>
<script>
new Vue({
  el: '#example-6',
  data: {
    selected: []
  }
})
</script>
{% endraw %}
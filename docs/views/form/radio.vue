<template>
<div class="ex-content">
    <div class="ex-card">
    <mark>
        <textarea class="ex-mark-text">
# Radio 单选框
> 简单的radio
 * 用于在多个备选项中选中单个状态。
 * 和 Select 的区别是，Radio 所有选项默认可见，方便用户在比较中选择，因此选项不宜过多。
        </textarea>
    </mark>
        <p>
            <rd-radio :radios="radios"></rd-radio>
        </p>
    <mark>
        <textarea class="ex-mark-text">
# API

## radios
承载多个 radio 对象的数组
```html
<rd-radio :radios="radios"></rd-radio>
```

```
radios: [{
    // radio 的选择状态:Boolean
    checked: false,
    // radio 的展示文字: String
    value: 'A'
}, {
    checked: false,
    value: 'B'
}]
```
        </textarea>
    </mark>
    <mark>
        <textarea class="ex-mark-text">
## 示例代码
```javascript
export default { 
  template: '<rd-radio :radios="radios"></rd-radio>'
  data () {
    return {
        radios: [{
            disabled: true,
            checked: false,
            value: '北京'
        }, {
            checked: false,
            value: '上海'
        }, {
            checked: false,
            value: '杭州'
        }, {
            checked: false,
            value: '成都'
        }]
    }
  },
  components: {
    rdCheckbox
  }
}
```
        </textarea>
    </mark>
    </div>
</div>
</template>
<script>
import { Mark } from '../index'
import {
    rdRadio
} from '../../../src/components/index'

export default {
    data () {
        return {
            radios: [{
                disabled: true,
                checked: false,
                value: '北京'
            }, {
                checked: false,
                value: '上海'
            }, {
                checked: false,
                value: '杭州'
            }, {
                checked: false,
                value: '成都'
            }]
        }
    },
    components: {
        rdRadio,
        Mark
    }
}
</script>
<template>
<div class="ex-content">
    <h2></h2>
    <div class="ex-card">
        <mark>
            <textarea class="ex-mark-text">
# Checkbox 多选框
简单的checkbox

## 用法
```javascript
export default {
       template: ‘<rd-checkbox :checkbox="checkbox"></rd-checkbox>’
        data () {
            return {
                checkbox: {
                    checked: false,
                    text: "我已阅读用户协议"
                }
            }
        },
        components: {
           rdCheckbox
        }
    }
```
## 示例
            </textarea>
        </mark>
        <p>
            <rd-checkbox :checkbox="checkbox"></rd-checkbox>
            <rd-checkbox :checkbox="checkA"></rd-checkbox>
        </p>
    </div>
</div>
</template>
<script>
import { Mark } from '../index'
import {
    rdCheckbox
} from '../../../src/components/index'

export default {
    data () {
        return {
            checkbox: {
                checked: false,
                text: '我已阅读用户协议'
            },
            checkA: {
                disabled: false,
                checked: false,
                text: '同意服务条款'
            }
        }
    },
    components: {
        rdCheckbox,
        Mark
    }
}
</script>
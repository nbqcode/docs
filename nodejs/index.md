---
hello: world
---

<script setup>
import { ref } from 'vue'
import { useData } from 'vitepress'

const { page } = useData()
const count = ref(0)
</script>

## Markdown Content

The count is: {{ count }}
{{page}}
<button :class="$style.button" @click="count++">Increment</button>

<style module>
.button {
  color: red;
  font-weight: bold;
}
</style>

```php
 echo "hello word";
```

## Selecting Values {#values}

The most common use case for `vue-select` is to have the chosen value synced with a parent component. `vue-select` takes advantage of the `v-model` syntax to sync values with a parent.

```html
<v-select v-model="selected"></v-select>
```

[](codepen://sagalbot/Kqxbjw?height=250)

If you don't require the `value` to be synced, you can also pass the prop directly:

```html
<v-select :value="selected"></v-select>
```

This method allows you to pre-select a value(s), without syncing any changes to the parent component. This is also very useful when using a state management tool, like Vuex.

### Single/Multiple Selection {#multiple}

By default, `vue-select` supports choosing a single value. If you need multiple values, use the `multiple` prop:

```html
<v-select multiple v-model="selected"></v-select>
```

[](codepen://sagalbot/opMGro?height=250)

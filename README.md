# vue-basics
#### Difference between v-model and v-bind:value
```html
<input v-model="something">
```
```html
<input
   v-bind:value="something"
   :value="something" (shorthand syntax)
   v-on:input="something = $event.target.value"
   @input="something = $event.target.value" (shorthand)
>
```
So v-model is a two-way binding for form inputs. It combines v-bind, which brings a js value into the markup, and v-on:input to update the js value.

Use v-model when you can. Use v-bind/v-on when you must.

v-model [works with all the basic HTML input types](https://vuejs.org/v2/guide/forms.html) (text, textarea, number, radio, checkbox, select).

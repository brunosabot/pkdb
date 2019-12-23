# Forms

## Contents

 - [Value reactivity](#value_reactivity)

## <a name="value_reactivity"></a>Value reactivity

When updating an input value from props, sometimes it just doesn't work when the input is already "dirty"

We can use `refs` to orce the input to update

```javascript
export default {
  watch: {
    value() {
      this.$refs.input.value = this.value;
    }
  },
};
```

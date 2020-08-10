# Slot

## Contents

- [Check if a slot is empty](#check_if_a_slot_is_empty)

## <a name="check_if_a_slot_is_empty"></a>Check if a slot is empty

A vNode child will be either:

- `tag` if content is a subcomponent or a dom element
- `text` if content is not subcomponent or a dom element

So we can check if the slot is falsy with this snippet

```javascript
export default {
  computed: {
    isSlotFalsy() {
      return (
        !this.$slots.default ||
        this.$slots.default.every((vNode) => !vNode.tag && !vNode.text)
      );
    },
  },
};
```

# Expect

## Contents

- [Match an object instance](#match_an_object_instance)

## <a name="match_an_object_instance"></a>Match an object instance

Jest has a function `expect.any` to match an instance of the object.

```javascript
const mock = jest.fn();
class MyObject {}

mock(new MyObject());

expect(mock).toHaveBeenCalledWith(expect.any(MyObject));
```

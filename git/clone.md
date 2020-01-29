# Clone

## Contents

 - [Clonable bundle](#clonable_bundle)

## <a name="clonable_bundle"></a>Clonable bundle

Using `git bundle`, we can create a clonable git bundle that we can send by mail.

The syntax is:

```shell
git bundle create your_name.bundle --all
```

Then, we can use the repository by cloning it:

```shell
git clone <path_to_bundle_file>
```

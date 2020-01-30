# Commands

## Contents

 - [Clonable bundle](#clonable_bundle)
 - [Push force with lease](#push_force_with_lease)

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

## <a name="push_force_with_lease"></a>Push force with lease

To avoid some commits to be ereased, we can use `--force-with-lease` instead of just `--force`.

It will ensure the remote version index is up to date in local so our collegue most recent commit will not be removed.

```shell
git push --force-with-lease
```

We can also add a .gitconfig alias to make it shorter

```
[alias]
    fpush = push --force-with-lease
```
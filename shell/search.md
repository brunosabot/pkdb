# Search

## Contents

 - [Exclude results from search](#exclude_results_from_search)

## <a name="exclude_results_from_search"></a>Exclude results from search

The `grep` method has a `-v` option to reverse the search

To find all files excluding the _node_modules_ folder, we can use

```shell
find . | grep -v node_modules
```

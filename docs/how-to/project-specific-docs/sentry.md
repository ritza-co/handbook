To count all the words recursively in a specific folder, you can use 

```
find . -type f -exec wc -w {} \; | tr -s ' ' | cut -d' ' -f 2 | paste -sd+ - | bc
```

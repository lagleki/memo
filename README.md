# memo

## replace recusrsively in all files

```
find /home/www/ -type f -exec \
    sed -i 'somesite\.com/anothesite.com/g' {} +
```

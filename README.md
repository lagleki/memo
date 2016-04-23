# memo

## replace recusrsively in all files

```
find /home/www/ -type f -exec \
    sed -i 'somesite\.com/anothesite.com/g' {} +
```
```
find . -type f \( -iname \*.css -o -iname \*.js -o -iname \*.json \) -not \( -path './.git/*' -o -path './node_modules/*' \) \
  -exec sed -i 'Statinamic/Phenomic/g' {} +
find . -type f \( -iname \*.css -o -iname \*.js -o -iname \*.json \) -not \( -path './.git/*' -o -path './node_modules/*' \) \
  -exec sed -i 'statinamic/phenomic/g' {} +
find . -type f \( -iname \*.css -o -iname \*.js -o -iname \*.json \) -not \( -path './.git/*' -o -path './node_modules/*' \) \
  -exec sed -i 'STATINAMIC/PHENOMIC/g' {} +
```

# memo

## replace recusrsively in all files

```
find /home/www -type f -print0 | xargs -0 sed -i 's/subdomainA.example.com/subdomainB.example.com/g'
```
```
find . -type f \( -iname \*.css -o -iname \*.js -o -iname \*.json \) -not \( -path './.git/*' -o -path './node_modules/*' \) \
  -exec sed -i 'Statinamic/Phenomic/g' {} +
find . -type f \( -iname \*.css -o -iname \*.js -o -iname \*.json \) -not \( -path './.git/*' -o -path './node_modules/*' \) \
  -exec sed -i 'statinamic/phenomic/g' {} +
find . -type f \( -iname \*.css -o -iname \*.js -o -iname \*.json \) -not \( -path './.git/*' -o -path './node_modules/*' \) \
  -exec sed -i 'STATINAMIC/PHENOMIC/g' {} +
```

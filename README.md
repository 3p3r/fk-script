# fk-script

"fk-script" is an experimental polyglot runtime and scripting language

## usage

> - install: `npm install -g fk-script`
> - run: `fks main.fk`
> - help: `fks --help`
> - uninstall: `npm uninstall -g fk-script`

## mvp

```PHP
<?fk python
from math import sqrt

def quadratic(a, b, c):
    x1 = -b / (2*a)
    x2 = sqrt(b**2 - 4*a*c) / (2*a)
    return (x1 + x2), (x1 - x2)
fk?>
// this is some comment in between
<?fk javascript
console.log(<?py quadratic(c=31, b=93, a=62) py?>);
fk?>
```

# Readable Random String PHP

A PHP Port of [@arnoclr](https://github.com/arnoclr) 's [Readable Random String](https://github.com/arnoclr/random-readable-string) for JS


Creates a random (as far as Math.random is random) string that is readable for humans.
This can be used to generate usernames or small links that can be more easily remembered.

Avoid using this for passwords, because it is not secure (generate strings contains only lowercase letters).

## usage

```php
include "RandomReadableString.php";

$rrs = new RandomReadableString();

$rrs->rrs(5);
// "uthek"
```

## parameters

#### `length`: number

Length of returned string.

#### `separatorGap`: number (default: 0)

Return string separated by dashes every `separatorGap` characters.

example :
    
```php
$rrs = new RandomReadableString();

$rrs->rrs(9, 4);
// "mela-ekou"
```

## Licence

Licensed under MIT license, Copyright © 2022 CELLARIER Arno & Mathieson Adam

# Env

Registers environment variables from a .env file (only 31 lines of code!)

## Installation

```bash
composer require vendor/env
```

## .env format (RAW)

```
#COMMENT
VAR=foo
```

## Use

```php
<?php
require 'vendor/autoload.php';

use devgaucho\Env;

$env_filename=__DIR__.'/.env';

new Env($env_filename);
print $_ENV['VAR'];//output: foo
```

# Laravel Shell Executor 


## Usage

Init
```bash
  copy class to your peject folder 
  Ex : app/services/ShellExecutor.php
```

Change namespace

```bash
  App\Helpers => YourNameSpace
  Ex : namespace App\Services
```

Bind class with the service container

```bash
  Go to AppServiceProvider 
  inside the boot function 
  add this code bellow 
```

```bash
$this->app->singleton(ShellExecutor::class, function () {
            return new ShellExecutor( realpath(__DIR__ . '/../../'));
});
```



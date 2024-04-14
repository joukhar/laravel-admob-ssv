# Laravel Google AdMob Server-side Verification
The library help you to verify Admob callback in server.

## Install
```
composer require joukhar/laravel-admob-ssv
```


## How to use

```php
use Joukhar\LaravelAdmobSsv\AdMob;
use Illuminate\Http\Request;

public function callback(Request $request) {
    $adMob = new AdMob($request);
    if ($adMob->validate()) {
        // success
    } else {
        // failed
    }
}
```

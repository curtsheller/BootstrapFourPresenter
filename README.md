#Laravel 5.1> Bootstrap 4 Presenter

Based on an article at: http://laravelista.com/laravel-custom-pagination-presenter/ and notes from around the web.

The render() method accepts an Illuminate\Contracts\Pagination\Presenter instance. You can create a custom class that implements that contract and pass it to the render() method.
    
#### Usage
```
$users = App\User::paginate(15);
{!! with(new \App\Services\Pagination\BootstrapFourPresenter($users))->render() !!}
```
#### License

This is free software distributed under the terms of the MIT license

#Installation

Require this package in your `composer.json` and run the `composer update` commmand. This will download the package and PHPExcel of PHPOffice.

    "maatwebsite/excel": "1.*"

After updating composer, add the ServiceProvider to the providers array in `app/config/app.php`

    'Maatwebsite\Excel\ExcelServiceProvider',

You can use the facade for shorter code. Add this to your aliases in `app/config/app.php`:

    'Excel' => 'Maatwebsite\Excel\Facades\Excel',

The class is bound to the ioC as `excel`

    $excel = App::make('excel');

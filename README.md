# SimpleSAMLphp Module: phpBB Auth
This is a module for SimpleSAMLphp that will allow you to use your phpBB forum as an authentication source.


## Configuration

Update your `config.php` file to make sure the module is enabled.

````
    'module.enable' => [
        'phpbbauth' => true,
         ....
     ];
````

Update your `authsources.php` file to add variables specific to your phpBB installation:

````
    'phpbb' => [
        'phpbbauth:PhpbbAuth',
        'phpbb_path' => '/path/to/your/forum/',
        'phpbb_dbms' => 'mysql', //Use mysql instead of mysqli
        'phpbb_dbhost' => 'localhost',
        'phpbb_dbport' => '',
        'phpbb_dbname' => 'YOUR DB NAME',
        'phpbb_dbuser' => 'YOUR DB USERNAME',
        'phpbb_dbpasswd' => 'YOUR DB PASSWORD',
        'phpbb_table_prefix' => 'phpbb3_',
    ],
````

## License

    The MIT License (MIT)

    Copyright (c) 2023 multidimension.al
	
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.

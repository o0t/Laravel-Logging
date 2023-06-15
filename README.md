
# Explain how Laravel Logging works



### Create your own logo [ config/logging.php ]

- [Document](https://laravel.com/docs/10.x/logging#building-log-stacks)



--------------------------

## Type 
    
- Log::emergency($message);

- Log::alert($message);

- Log::critical($message);

- Log::error($message);

- Log::warning($message);

- Log::notice($message);

- Log::info($message);

- Log::debug($message);


----

## EX 

    throw new Exception("Hello Log ");


    Log::info('User {id} failed to login.', ['id' => $user->id]);


----

## Log file path 

     Storage/logs/FileName.log



## EX 

    Log::channel('slack')->info('Something happened!');

----

    Log::channel('custom')->critical("Hello Log");;

----

    App::abort(403, 'Unauthorized testing.');




### Laravel Queues

1. change .env
```
QUEUE_DRIVER=database
```
2. run
```shell
php artisan queue:table
php artisan migrate
 ```
3. to create job, run (file created at app\jobs)
```shell
php artisan make:job <job_name>
```
4. to start queue, run
```shell
php artisan queue:work
```
5. try trigger the queue

note: install Supervisor to start queue:work automatically
```shell
sudo apt-get install supervisor
```
Official Documentation
- [Laravel Queues Documentation](https://laravel.com/docs/5.4/queues)
- [Queues Tutorial](https://scotch.io/tutorials/why-laravel-queues-are-awesome)

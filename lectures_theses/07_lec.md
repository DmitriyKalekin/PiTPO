**Блокирующие операции** 
-- файловые операции  
-- подключение сокета  
-- получение данных из сокета  

Переключение потоков = накладные расходы OVERHEAD   
~~ 5мс на переключение  
[https://metanit.com/sharp/tutorial/11.1.php]  
Свойство IsBackground указывает, является ли поток фоновым   
- какой поток называется фоновым?  
ThreadStart и без него  
[https://metanit.com/sharp/tutorial/11.2.php] 
[https://docs.microsoft.com/ru-ru/dotnet/api/system.threading.thread.start?view=netframework-4.8]  
[https://metanit.com/sharp/tutorial/11.3.php]

**Общие ресурсы** - БОЛЬ  
lock (locker) - позволяет организовать общий доступ к ресурсам  
Deadlock - ситуация когда оба потока ждут ресурса, захваченного другим потоком  
[https://metanit.com/sharp/tutorial/11.4.php]
[https://metanit.com/sharp/tutorial/11.5.php]
[https://metanit.com/sharp/tutorial/11.7.php]
[https://metanit.com/sharp/tutorial/11.8.php]


**Pool of workers** 
```
object[] threads = new object[20]();

while (!threads.Contains(null))
{
  int i = threads.Index(null)
  threads[i] = new Thread(do_work);
  threads[i].Start();
  
  for (int i=0; i<20; i++)
  {
    if (! threads[i].IsAlive)
    {
      threads[i].Join();
      threads[i] = null;
    }
  }
    
}
```


**Tasks**   
[https://metanit.com/sharp/tutorial/12.1.php]
[https://metanit.com/sharp/tutorial/12.2.php]




**Асинхронность**  
[https://metanit.com/sharp/tutorial/13.3.php]
...Async

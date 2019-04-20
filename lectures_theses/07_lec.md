Блокирующие операции
-- файловые операции
-- подключение сокета
-- получение данных из сокета

Переключение потоков = накладные расходы OVERHEAD
~~ 5мс на переключение

Свойство IsBackground указывает, является ли поток фоновым

Общие ресурсы - БОЛЬ
lock (locker)
        {
        }
        
Deadlock
Tasks


//  Pool of workers
threads[20] === null*20

while null not in threads
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














Асинхронность
...Async

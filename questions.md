1.Архитектура .NET  
CTS – Common Type System  
Garbage Collector  
MSIL – Microsoft Intermediate Language  
Assembly / Namespace  C:\Windows\Assembly  

2. Типы данных. Преобразование типов. Boxing & unboxing  
Значимые типы: целое, вещественное, булево.  
Ссылочные типы: классы, делегаты.  

Куда отнести: структуры, списки, массивы и строки? 

int Int32

```
Convert  
int.Parse   
bool int.TryParse(… out val) // ref out  
*.ToString()  

int a = (int)(5/2);  
Planet p = new Planet();  

// public void Process(object a, object b)  

*.Process((object)p, (object)a); // Boxing

object o = (object)p;
Planet p2 = (Planet)o; // UnBoxing

instanceof  ==> is

class SpaceObject // x,y, name, Process()
class Planet : SpaceObject // R, star, 
class Comet : SpaceObject

*.Render(new Planet());

public void Render(SpaceObject so)
{
	// so – Не будет R и star – потому что их нет в SpaceObject

	if(so is Planet){
		Planet p = (Planet)so;
		p.Process();
}



.GetType(???) == “\Lab2\Planets\SpaceObject”
typeof(i) == int
```

3. UML. Class Diagram + Основы ООП
Инкапсуляция – содержать в себе данные и методы, но и защитить  
Наследование  
Полиморфизм  
Модификаторы доступа: public+, private-, protected#  
Делегирование, делегация (не путать с делегатом, или можно путать))))  
Композиция, агрегация
Реализация инерфейса
Ассоциация (класс ассоциация)
Делегирование

4.	Паттерны проектирования  
Типы: Поведенческие, Порождающие, Корпоративных приложений, …  
Strategy / Bridge  
Factory / Abstract Factory / Factory Method  
Singleton –  Config, MySQL_Connector  
Builder  
Composite  
Фасад  
Декоратор  
Front Controller  
Page Controller  
Observer / Subscriber / Listener  

5. Теория вычислимости. Сложность алгоритмов  
О(N), o(N), Omega(N)  

O(N) = O(cN)   
O(N*logN) O(N^k)  

log A B = log c B /  log c A


P, NP  

Комбинаторика: сочетания, размещения  
-- перебор всех сочетаний или размещений  

```
for (int i=0; i<N; i++)
	for (int j=i+1; j<N; j++)
		for (int k=j+1; k<N; k++)
			print(I, j, k);
```

6.Сортировки сдвигом, быстрая, пузырьковая, Хоара  


7.События, обработка событий, делегаты и шаблон Observer/Listener/Наблюдатель   


8.
Устар: восходящее и нисходящее программирование
Процедурное программирование
Основы функционального программирования.   
Fluent Interface. 
LINQ. Лямбда-выражения   
Когда функция возвращает функцию?


9.IEnumerable, IEnumerator, Генератор, yield return, Lazy Loading   

10.MVC, MVP, MVVM  


13. Потоки и Процессы 
Thread, join. Worker, BackgroundWorker  

14. Сериализация и маршалинг  
Binary, XML  
 
15. Файлы Stream
StreamReader / Writer / ... binary... xml
Как проверить, что файл существует?
Обойти рекурсивно каталог и отобразить файлы и папки (и содержимое внутренних каталогов)
Записать в файл, прочитать

---------------------------------------------
Подключение DLL
Копирование/клонирование объектов. Поверхностное (shallow) и глубокое (deep) копирование

** проектирование **  
SOLID  
DRY  

** тестирование **  
TDD
Mock, Stub
BDD (cucumber, gherkins)
DDD

Функциональное тестирование (selenium)

Модульное тестирование


** практическое **
1. изменение размера массива
2. удаление i-го элемента в списке
3. исключить элемент из списка / вернуть список, не содержащий элемент E
4. перемножение матриц
5. обход графа вглубь
6. определение существования цикла в графе
7. реализовать алгоритм сортировки (любой)






------------ не будет ------------------
11. Параметрическая оптимизация. Метод градиентного спуска.  

12. Постановка задачи Машинного обучения – любой  
-- либо классификация, либо регрессия  
Воронцов (Яндекс Youtube)  
Andrew Ng (Coursera.Org – Stanford – Machine Learning)  









































	

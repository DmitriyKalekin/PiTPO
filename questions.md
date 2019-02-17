1.Архитектура .NET  
CTS – Common Type System  
Garbage Collector  
MSIL – Microsoft Intermediate Language  
Assembly / Namespace  C:\Windows\Assembly  

2. Типы данных. Преобразование типов. Boxing & unboxing  
Значимые типы: целое, вещественное, булево.  
Ссылочные типы: классы, делегаты.  

Куда отнести: структуры, списки, массивы и строки?  

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
typeof() == int
```

3. UML. Class Diagram + Основы ООП
Инкапсуляция – содержать в себе данные и методы, но и защитить  
Наследование  
Полиморфизм  

Модификаторы доступа: public+, private-, protected#  

Делегирование, делегация (не путать с делегатом, или можно путать))))  

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


8.Fluent Interface. Основы функционального программирования.   
LINQ. Лямбда-выражения   

9.IEnumerable, IEnumerator, Генератор, yield return, Lazy Loading   

10.MVC, MVP, MVVM  

11. Параметрическая оптимизация. Метод градиентного спуска.  

12. Постановка задачи Машинного обучения – любой  
-- либо классификация, либо регрессия  
Воронцов (Яндекс Youtube)  
Andrew Ng (Coursera.Org – Stanford – Machine Learning)  

13. Потоки  
Thead, join. Worker, BackgroundWorker  

14. Сериализация и маршалинг  
Binary, XML  
 
















	

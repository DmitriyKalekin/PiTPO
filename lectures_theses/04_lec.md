

||


if (file_exists(f) && readfile(f).size > 0) 
{


}


class SpaceObject {

	public virtual void Process(double t)
	{
		...
	}

}

class Planet : SpaceObject {

	public override void Process(double t)
	{
		...
	}

}



class Estate {


	public IEnumerator GetEnumerator()
        {
            for(int i = 0; i < 6; i++)
            {
                yield return i * i;
            }
        }


	Room this[int index] {


	}

}




class  Library {

	Book[] getAllBooks() {
		return 2GB of books....
	}
}

Library l = new Library();

foreach (Book b in l.getAllBooks())
{
	...
}

















Estate dom = Estate();

foreach (Room r in dom)
{

}

dom[5]

for (int i=0; i < 5; i++)
{
	... dom[i]

}



















class Estate {
	protected double price;
	protected double square;
	protected double ppsm;



	[Property defaultValue=5 .... ]
	public double Price {
		get {
			return this.price;
		}
		set {
			this.price = value;
			this.ppms = this.price / this.square;
		}

	}



	// getter
	public double getPrice(){
		return this.price;
	}

	// setter
	public void setPrice(double value){
		this.price = value;
		try {
		this.ppsm = this.price / this.square;
		} 
		catch Exception e
		{

		}
	}

	
	
}

Estate dom = new Estate();
dom.price = 5;
dom.square = 500;

...
...
..
dom.ppsm = 30;

dom.Price = 7;
Console.WriteLine(dom.Price);



class SpaceObject {
	public virtual void Process(){
	}
}


class Planet : SpaceObject  {
	public override void Process(){
	}
}


class Data {
	public List<int> getData(){...}
}


Data d = new Data();

foreach (int a in d.getData())
{
	a = d.getNext()

}



Pattern LazyLoading




class NewController {

	public process_Index() {
		ModelNews m = new ModelNews();
		NewsCollection news = m.LoadNews(); // ALL!!!

		ViewNews page = new ViewNews();
		return page.render(news, "Heading!");
	}



}

class ModelNews{
	private MySQLConnection connection = null;

	public ModelNews(){
		this.connection  = Mysql.Connect(
				"127.0.0.1",
				"root",
				"123",
				"test_db"
			)

	}



}









class DBConn {

	private static instance = null;

	private DBConn(){}

	public static DBConn getInstance(){
		if (this.instance == null)
		{
			this.instance = new self();
			return this.instance ;
		}
		else {
			return this.instance;	
		}

	}



}


// DBConn c = new DBConn();

DBConn d = DBConn.getInstance();

// ....
DBConn ddd = DBConn.getInstance();





































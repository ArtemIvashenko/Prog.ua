package mars;

public class Main {

	public static void main(String[] args) {
		Mars mars = new Mars("Mars", 2,15);
		
		mars.print();
		mars.go();
		mars.stop(5);
		
		Mars dog = new Mars ("Tayson", 5, 43);
		dog.print();
		dog.voice();
		dog.stop(0);
	}

}
package mars;

public class Mars {
	private String name;
	private int old;
	private int weight;
	private int speed = 0;

	public Mars(String name, int old, int weight) {
		super();
		this.name = name;
		this.old = old;
		this.weight = weight;
	}

	public String getName() {
		return name;
	}

	public void setName(String name) {
		this.name = name;
	}

	public int getOld() {
		return old;
	}

	public void setOld(int old) {
		this.old = old;
	}

	public int getWeight() {
		return weight;
	}

	public void setWeight(int weight) {
		this.weight = weight;
	}
public void go(){
	System.out.println("Собака идет");
}
public void voice(){
	System.out.println("lay");
}
public void stop(int a){
	if (a<=speed){
		System.out.println("Собака сидит");
		}
		else {
			System.out.println("Собака идет со скоростью  "+ a + " m/h");
		}
	}
public void print(){
	System.out.println("Name "+name);
	System.out.println("Old "+ old);
	System.out.println("Weight "+ weight);
}
}

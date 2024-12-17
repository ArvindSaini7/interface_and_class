# interface_and_class
use factory methods
package clas_in_interface;

interface RbiBank{
	void interest();
}


public class Sbi_bank implements RbiBank{
	
	public void interest() {
		System.out.println("12%");
		}
}
package methods_factory;
import clas_in_interface.Sbi_bank;
public class Sbi_factory {
	public static  Sbi_bank getobj() {
		return new Sbi_bank();
	}

}
package main_class;
import clas_in_interface.Sbi_bank;
import methods_factory.Sbi_factory;
public class Sbi_main {
	public static void main(String[]args) {
		Sbi_bank id=Sbi_factory.getobj();
		id.interest();
	}
	

}

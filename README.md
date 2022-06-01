# Java_schoolProject
객체지향_과제(쇼핑)
import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		Scanner scanner=new Scanner(System.in);
		System.out.println("쇼핑하실 카테고리의 번호를 눌러주세요. 1.옷 2.악세서리 3.화장품 /n *쇼핑을 원하지 않으시면 다른 키를 눌러주세요*");
		String shoppingNumber=scanner.next();		//쇼핑할 카테고리 번호 입력받기
		Shopping shopping;		
		
		while(true) {
		
			if(shoppingNumber=="1") {
				shopping=new Clothes();
				shopping.shoppingChoose();
								//System.out.println(shopping.total);
			}
			else if(shoppingNumber=="2") {
				shopping=new Accessory();
				shopping.shoppingChoose();
								//System.out.println(shopping.total);
			}
			else if(shoppingNumber=="3") {
				shopping=new Cosmetic();
				shopping.shoppingChoose();
								//System.out.println(shopping.total);
			}
			else {
        breaak;
			}

			
		}
		
		
	}
}

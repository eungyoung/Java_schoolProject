import java.util.Scanner;

public class Accessory extends Shopping{
	
	public int total;
	public Accessory() {};
	public Accessory(String shoppingNumber) {};

	public void shoppingChoose() {
		while(true) {
			System.out.println("구매하실 상품의 번호를 입력하세요./n 1.목걸이 2.귀걸이 3.팔찌 4.반지/n *옷 구매 종료를 원하시면 1,2를 제외한 키를 눌러주세요.*");
			Scanner scan=new Scanner(System.in);
			String AccessoryNumber=scan.next();
			if (AccessoryNumber=="1"){
				System.out.println("구매하실 목걸이의 번호를 입력하세요./n 1.은목걸이(5000원) 2.써지컬목걸이_각인x(10000원) 3.써지컬목걸이_각인o(15000원) 4.금목걸이(20000원)");
				String necklace=scan.next();
				if(necklace=="1") {
					total+=5000;
					}
				else if(necklace=="2") {
					total+=10000;
					}
				else if(necklace=="3") {
					total+=15000;				
					}
				else if(necklace=="4"){
					total+=20000;
					}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}
			}
			else if(AccessoryNumber=="2") {
				System.out.println("구매하실 귀걸이의 번호를 입력하세요./n 1.은귀걸이(10000원) 2.써지컬(15000원) 3.금귀걸이(20000원)");
				String earringNumber=scan.next();
				if(earringNumber=="1") {
					total+=10000;
					}
				else if(earringNumber=="2") {
					total+=15000;
					}
				else if(earringNumber=="3") {
					total+=20000;				
					}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}
			}
			else if(AccessoryNumber=="3") {
				System.out.println("구매하실 팔찌의 번호를 입력하세요./n 1.은팔찌(5000원) 2.써지컬팔찌_각인x(10000원) 3.써지컬팔찌_각인o(15000원) 4.금팔찌(20000원)");
				String braceletNumber=scan.next();
				if(braceletNumber=="1") {
					total+=5000;
				}
				else if(braceletNumber=="2") {
					total+=10000;
				}
				else if(braceletNumber=="3") {
					total+=15000;
				}
				else if(braceletNumber=="4") {
					total+=20000;
				}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}						
			}
			else if(AccessoryNumber=="4") {
				System.out.println("구매하실 반지의 번호를 입력하세요./n 1.아크릴반지(4000원) 2.비즈반지(7000원) 3.써지컬반지_각인x(10000원) 4.써지컬반지_각인o(15000원)");
				String ringNumber=scan.next();
				if(ringNumber=="1") {
					total+=4000;
				}
				else if(ringNumber=="2") {
					total+=7000;
				}
				else if(ringNumber=="3") {
					total+=10000;
				}
				else if(ringNumber=="4") {
					total+=15000;
				}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}
			}
			else {
				break;
			}						
			
		}
	}

	
	
	
	
}


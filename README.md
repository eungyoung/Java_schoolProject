import java.util.Scanner;

public class Cosmetic extends Shopping{
	
	public int total;
	public Cosmetic() {};
	public Cosmetic(String shoppingNumber) {};
	public void shoppingChoose() {
		while(true) {
			System.out.println("구매하실 상품의 번호를 입력하세요./n 1.기초 2.베이스 3.색조 /n *옷 구매 종료를 원하시면 1,2를 제외한 키를 눌러주세요.*");
			Scanner scanner=new Scanner(System.in);
			String cosmeticNumber=scanner.next();
			if (cosmeticNumber=="1"){
				System.out.println("구매하실 기초화장품의 번호를 입력하세요./n 1.스킨(7000원) 2.로션(10000원) 3.수분크림(15000원) 4.아이크림(20000원)");
				String skinNumber=scanner.next();
				if(skinNumber=="1") {
					total+=7000;
				}
				else if(skinNumber=="2") {
					total+=10000;
				}
				else if(skinNumber=="3") {
					total+=15000;				
				}
				else if(skinNumber=="4"){
					total+=20000;
				}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}
			}
			else if(cosmeticNumber=="2") {
				System.out.println("구매하실 베이스화장품의 번호를 입력하세요./n 1.파운데이션(15000원) 2.파우더(12000원) 3.하이라이터(10000원) 4.셰이딩(10000원) 5.블러셔(8000원)");
				String baseNumber=scanner.next();
				if(baseNumber=="1") {
					total+=15000;
				}
				else if(baseNumber=="2") {
					total+=12000;
				}
				else if(baseNumber=="3") {
					total+=10000;				
				}
				else if(baseNumber=="4") {
					total+=10000;
				}
				else if(baseNumber=="5") {
					total+=8000;
				}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}
			}
			else if(cosmeticNumber=="3") {
				System.out.println("구매하실 색조화장품의 번호를 입력하세요./n 1.아이브로우(7000원) 2.아이라이너(10000원) 3.아이섀도우(15000원) 4.립스틱(17000원)");
				String colorNumber=scanner.next();
				if(colorNumber=="1") {
					total+=7000;
				}
				else if(colorNumber=="2") {
					total+=10000;
				}
				else if(colorNumber=="3") {
					total+=15000;				
				}
				else if(colorNumber=="4") {
					total+=17000;
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

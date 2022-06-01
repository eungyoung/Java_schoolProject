import java.util.Scanner;

public class Clothes extends Shopping{
	
	public int total;
	public Clothes(){};
	public Clothes(String shoppingNumber) {}
	@Override
	public void shoppingChoose() {
		while(true) {
			System.out.println("구매하실 상품의 번호를 입력하세요./n 1.상의 2.하의 /n *옷 구매 종료를 원하시면 1,2를 제외한 키를 눌러주세요.*");
			Scanner scanner=new Scanner(System.in);
			String clothNumber=scanner.next();
			if (clothNumber=="1"){
				System.out.println("구매하실 상의의 번호를 입력하세요./n 1.반팔티(5000원) 2.긴팔티(10000원) 3.블라우스(15000원) 4.셔츠(20000원)");
				String topNumber=scanner.next();
				if(topNumber=="1") {
					total+=5000;
					}
				else if(topNumber=="2") {
					total+=10000;
					}
				else if(topNumber=="3") {
					total+=15000;				
					}
				else if(topNumber=="4"){
					total+=20000;
					}
				else {
					System.out.println("번호를 잘못 입력하셨습니다. 다시 입력해주세요.");
					continue;
				}
			}
			else if(clothNumber=="2") {
				System.out.println("구매하실 하의의 번호를 입력하세요./n 1.반바지(5000원) 2.긴바지(10000원) 3.미니스커트(5000원) 4.롱스커트(10000원)");
				String bottomNumber=scanner.next();
				if(bottomNumber=="1") {
					total+=5000;
					}
				else if(bottomNumber=="2") {
					total+=10000;
					}
				else if(bottomNumber=="3") {
					total+=5000;				
					}
				else if(bottomNumber=="4") {
					total+=10000;
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
		// TODO Auto-generated method stub
		
	}
	
	
	

}

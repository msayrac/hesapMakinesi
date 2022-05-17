# hesapMakinesi
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        int number1, number2, select;


        Scanner input = new Scanner(System.in);

        System.out.println("İlk sayiyi giriniz : ");

        number1 = input.nextInt();

        System.out.println("ikinci sayiyi giriniz : ");
        number2 = input.nextInt();

        System.out.println("1-Toplama\n2-cikarma\n3-carpma\n4-bolme");

        System.out.println("Seciminizi yapiniz : ");

        select = input.nextInt();


        switch (select) {
            case 1:
                System.out.println("toplam : " + (number1 + number2));
                break;
            case 2:
                System.out.println("cikarma : " + (number1 - number2));
                break;
            case 3:
                System.out.println("carpma : " + (number1 * number2));
                break;
            case 4:

                if (number2 != 0) {
                    System.out.println("bolme : " + (number1 / number2));

                } else {
                    System.out.println("Sayi Sıfıra bölünemez");
                }
                break;
            default:
                System.out.println("1-4 arası secim yapiniz");
        }
    }
}

import java.util.Scanner;

public class Main2 {

    public static void main(String[] args) {
    
    //Girilen 3 sayıyı "küçükten büyüğe" sıralayan programı yazınız.

        int a,b,c;
        Scanner input= new Scanner(System.in);

        System.out.print("1. sayıyı giriniz: ");
        a= input.nextInt();

        System.out.print("2. sayıyı giriniz: ");
        b= input.nextInt();

        System.out.print("3. sayıyı giriniz: ");
        c= input.nextInt();

        if(a<b && a<c)
        {
            if(b<c){
                System.out.print("a<b<c");
            } else if (c<b) {
                System.out.print("a<c<b");

            }
        } else if (b<c && b<a) {
            if(c<a){
                System.out.print("b<c<a");
            } else if (a<c) {
                System.out.print("b<a<c");

            }

        } else if (c<a && c<b) {
            if(a<b){
                System.out.print("c<b<a");
            } else if (b<a) {
                System.out.print("c<a<b");

            }
        } else if (c==a || c==b || b==a) {
            System.out.print("Sayıları tekrardan giriniz");

        }


    }
}

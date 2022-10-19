# Recursive-Asal-Sayi-Bulma
---
Bu bir [patika.dev](www.patika.dev) projesidir.
```
import java.util.Scanner;
public class recursiveAsal {
    static void isAsal(int sayi,int i){
        if (i == sayi) {
            System.out.print(sayi + " asal sayıdır.");
            return;
        } else if (sayi%i == 0) {
            System.out.print(sayi + " asal sayı değildir.");
            return;
        }

        isAsal(sayi, i + 1);
    }

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Sayı giriniz: ");
        int sayi=input.nextInt();

        isAsal(sayi,2);
    }
}
```

# factorial

package Exercise;

import java.util.Scanner;

public class kombinasyon {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        long i, n, r, C, f, f2, f3;

        System.out.println("C(n,r)");
        System.out.print("n değerini giriniz : ");
        n = input.nextInt();
        System.out.print("r değerini giriniz : ");
        r = input.nextInt();
        f = 1;
        f2 = 1 ;
        f3 = 1;


        for (i = 1; i <= n; i++) {
            f *= i;
        }
        for (i = 1; i <= r; i++) {
            f2 *= i;

        }
        for (i = 1; i <= (n - r); i++) {
            f3 *= i;
        }


        C = f / (f2 * f3);
        System.out.println("Kombinasyon : " + C);

    }
}

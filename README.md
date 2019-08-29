# bubble-sorting
Сортировка методом пузырька
package пузырек;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class Пузырек {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        int i;
        System.out.println("vvedite razmer massiva: ");
        Scanner sc = new Scanner(System.in);
        int n=sc.nextInt();
        System.out.println("vvedite elementi massiva: ");
        int[] mas=new int[n];
        
        for (i=0; i<n; i++){
            mas[i]=sc.nextInt();
        }
        
        int b;
        int j;
       for(j=0; j<n-1; j++){
        for(i=0; i<n-1-j; i++)
        {
        if (mas[i+1]<mas[i]){
            b=mas[i];
            mas[i]=mas[i+1];
            mas[i+1]=b;
            }
        }
       }
        System.out.println("Sortirov. massiv: ");
        for( i=0; i<n; i++) {                  
                   System.out.print(mas[i]+" ");
    } 
    
}
}

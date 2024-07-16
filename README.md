# MAX-DIFFERENCE-IN-SUCCESSIVE-ELEMENTS-OF-ARRAY
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        int a[];
        a=new int[100];
        int c=0;
        Scanner sc= new Scanner(System.in);
        int n=sc.nextInt();// Array length
        for(int i=0;i<n;i++){
            int k=sc.nextInt();
            a[i]=k;
        }
        c=a[0]-a[1];
        for (int i=0;i<n-1;i++){
            if((a[i]-a[i+1])>c){
                c=a[i]-a[i+1];
            }
        }
        System.out.println(c+" IS MAX DIFFERENCE");
    }
}

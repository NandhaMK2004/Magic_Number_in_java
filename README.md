import java.util.Scanner;
public class Main{
    public static void main(String[]args){
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        int temp=a;
        int sum=0;
        int rev=0;
        while(a!=0){
            int last=a%10;
            sum+=last;
            a/=10;
        }
        int x=sum;
        while(x!=0){
            int last=x%10;
            rev=rev*10+last;
            x=x/10;
        }
        if(sum*rev==temp){
            System.out.println("Magic Number");
        }
        else{
            System.out.println("Not a Magic Number");
        }
    }    
}

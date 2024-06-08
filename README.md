# JAVA-program-to-check-armstrong-number
import java.util.Scanner;
public class armstrong
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        int temp=num;
        int sum=0;
        while(temp>0)
        {
            int digit=temp % 10;
            sum+=Math.pow(digit,3);
            temp=temp/10;
        }
        if(num==sum)
        {
            System.out.println(num+" is a armstrong number");
        }
        else
        {
              System.out.println(num+"is not a armstrong number");
        }
    }
}

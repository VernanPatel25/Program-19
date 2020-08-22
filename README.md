import java.util.*;
class Series2
{
    int n,S=0;
    void getData()
    {
        Scanner sc=new Scanner(System.in);
        n=sc.nextInt();
    }
    void calc()
    {
        for(int i=1;i<=n;i++)
        {
            int j;
            if(i%2!=0)
            {
                j=-i;
            }
            else
            {
                j=i;
            }
            S-=j;
        }
    }
    void disp()
    {
        System.out.println(S);
    }
    public static void main()
    {
        Series2 obj=new Series2();
        obj.getData();
        obj.calc();
        obj.disp();
    }
}

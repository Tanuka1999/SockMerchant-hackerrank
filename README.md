import java.util.*;
public class cp{
    public static void main(String args[])
  {
    int n,i,pair=0,count=1,j;
    int arr[]=new int[100];
    Scanner in=new Scanner(System.in);
    n=in.nextInt();
    for(i=0;i<n;i++)
    {
        arr[i]=in.nextInt();
    }
    for(i=0;i<n;i++)
    {
        for(j=i+1;j<n;j++)
        {
        if(arr[i]==arr[j])
        count++;
    }
    if(count%2==0)
    {
    pair++;
    count=1;
}
}
System.out.println(pair);
}
}


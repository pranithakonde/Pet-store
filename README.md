# Pet-store
import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner s = new Scanner(System.in); 
		int t = s.nextInt(); 
		for(int i =0;i<t;i++) 
		{ 
		    int n = s.nextInt();
		    int j;
		    int[] a =new int[n];
		    for(int k=0;k<n;k++)
		    {
		        a[k]=s.nextInt();
		    }
		    Arrays.sort(a);
		    if(n%2!=0)
		        System.out.println("NO");
		    else
		    {
		        for( j=0;j<n;j+=2)
		        {
		            if(a[j]!=a[j+1])
		            {   System.out.println("NO");
		                break;
		            }
		        }
		        if(j==n)
		            System.out.println("YES");
		    }
		}
	}
}

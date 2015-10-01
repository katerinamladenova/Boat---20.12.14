# Boat---20.12.14
From exam
using System;
					
public class Boat
{
	public static void Main()
	{
		int n = int.Parse(Console.ReadLine());
		int a = 0;
		int b = 1;
		
		
		for (int i = 0; i <= n; i++)
			{
			Console.WriteLine("{0}{1}{2}", new string('.', (n-1)-a), new string ('*', b), new String('.', n));
				i++;b+=2;a+=2;
			}
		a = 2;
		b = 1;
					
		for (int m = 0; m < n-1; m++)
			{
			Console.WriteLine("{0}{1}{2}", new string('.', a), new string ('*', n-a), new String('.', n));
				m++;b+=2;a+=2;
			}
		
		b = 0;
		a = 0;
				
		for (int i = 0; i < (n-1)/2; i++)
			{
				Console.WriteLine("{0}{1}{0}", new string ('.', b), new string('*', ((n*2))-a));
				b++;a+=2;
			}
			
	}
}

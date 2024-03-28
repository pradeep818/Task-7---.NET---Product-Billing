class System
{
    public static void Main(string[] args)
    {
        String[] a=new String[5];
        string[] m = new string[5];
        int[] v=new int[5];
        
        Console.ForegroundColor = ConsoleColor.Green;
        Label:
        Console.WriteLine("                  ****Welcome to Pradeep Mart****");
        Console.Write(" Are you a user or admin (0/1) :");
        int o=Convert.ToInt32(Console.ReadLine());
        if(o==1)
        {
            Console.ForegroundColor = ConsoleColor.Red;
            Console.WriteLine("            ****Welcome to Admin Login****");
            Console.ForegroundColor = ConsoleColor.Gray;
            Console.WriteLine("your User ID is : admin");
            Console.WriteLine(" your Password is : admin");
            Thread.Sleep(3000);
            Console.Clear();
            Console.Write("enter the password to set :");
            int s=Convert.ToInt32(Console.ReadLine());
            Console.ForegroundColor= ConsoleColor.Green;
            Console.WriteLine("           ****Please login by using password****");
            Console.WriteLine(" your User Id is : admin");
            Console.Write(" your password : ");
            int l=Convert.ToInt32(Console.ReadLine());  
            if(l==s)
            {
                Console.ForegroundColor = ConsoleColor.Blue;
                Console.Write(" Do you want add or create the products then click 1 : ");
                int j=Convert.ToInt32(Console.ReadLine());
                if(j==1)
                {
                    Console.ForegroundColor = ConsoleColor.Yellow;
                    Console.Write(" enter the no of items you want to add : ");
                    int  n=Convert.ToInt32(Console.ReadLine());
                    for(int i=0; i<n; i++)
                    {
                        Console.ForegroundColor = ConsoleColor.Magenta;
                        Console.Write(" enter your " + i + "item :  ");
                        a[i]=Console.ReadLine();
                        Console.Write("enter the cost of" +""+ i + "item :");
                        v[i] = Convert.ToInt32(Console.ReadLine());
                    }
                    Console.WriteLine("           *****Your Created List*****");

                    for (int i = 0; i < n; i++)
                    {
                        Console.WriteLine("Item :"+a[i]+"  "+"cost :" + v[i]);

                    }
                    Console.Write(" Are you a user or admin (0/1) :");
                    int d = Convert.ToInt32(Console.ReadLine());
                    if (d == 0)
                    {
                        Console.Clear();
                        Console.WriteLine("           *****list*****");
                        for (int i = 0; i < n; i++)
                        {
                            Console.WriteLine("item"+i+":"+a[i]+"    "+"cost :" + v[i]);
                            
                        }
                        Console.Write(" pick your no items :");
                        int z= Convert.ToInt32(Console.ReadLine());
                        if(n==z)
                        {
                            for (int i = 0; i < z; i++)
                            {
                                Console.Write(" enter your " + i + "item :  ");
                                m[i] = Console.ReadLine();
                                if (m[i] == a[i])
                                {
                                    Console.WriteLine(" item " + i + ":" +"cost :"+ v[i]);
                                }
                            }
                            Console.Clear();
                            Console.WriteLine("           *****Billing*****");
                            Console.Write(" Name :");
                            String x = Console.ReadLine();
                            Console.Write("Mobile No:");
                            int c = Convert.ToInt32(Console.ReadLine());
                            Console.WriteLine();
                            Console.WriteLine("Your ID :" + x + "PM");
                           int q = v[0] + v[1] + v[2] + v[3] + v[4] ;
                            Console.WriteLine("Total :" + q);

                        }


                    }


                }
                


            }
            if (l != s)
            {
                Console.ForegroundColor = ConsoleColor.Red;
                for (int i = 1; i <=3; i++)
                {
                    if (i == 2)
                    {
                        Console.WriteLine(" Alert Some unauthorized person is trying to open");
                    }
                    if (i == 3)
                    {
                        break;
                    }

                    Thread.Sleep(3000);
                    Console.Write(" Re enter your password :" + i + "attempt");
                    int u = Convert.ToInt32(Console.ReadLine());
                   

                }
            }

        }
        if(o==0)
        {
            int[] f = new int[5];
            int[] r=new int[5] { 123,456,765,434,242 };
            Console.WriteLine("123-->rice");
            Console.WriteLine("456-->dal");
            Console.WriteLine("765-->drink");
            Console.WriteLine("434-->bingo");
            Console.WriteLine("242-->chocolate");
            Console.WriteLine(); 
            Console.WriteLine("1." + r[0] + " " + "cost :" + r[0] * 2);
            Console.WriteLine("2." + r[1] + " " + "cost :" + r[1] * 2);
            Console.WriteLine("3." + r[2] + " " + "cost :" + r[2] * 2);
            Console.WriteLine("4." + r[3] + " " + "cost :" + r[3] * 2);
            Console.WriteLine("5." + r[4] + " " + "cost :" + r[4] * 2);
            Console.WriteLine();
            Console.Write(" pick your items :");
            int k = Convert.ToInt32(Console.ReadLine());
            for(int i = 1;i<=k;i++)
            {
                Console.Write("item" + i + ":");
                f[i]= Convert.ToInt32(Console.ReadLine());
                    

                
            }
            Console.WriteLine("               *****Billing*****");
            Console.Write(" Name :");
            String y = Console.ReadLine();
            Console.Write("Mobile No :");
            int z= Convert.ToInt32(Console.ReadLine()); 
            Console.WriteLine();
            Console.WriteLine("Your ID :"+y+"PM");
            
            int g = f[0]*2 + f[1]*2 + f[2]*2 + f[3] * 2 + f[4] * 2;
            Console.WriteLine();
            Console.WriteLine("Total : " + g);



        }
    }
}

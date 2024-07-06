import java.text.SimpleDateFormat;
import java.util.Date;
import java.util.Scanner;
import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;
class Task implements Runnable
{
    private String name;

    public Task(String s)
    {
        name = s;
    }


    public void run()
    {
        try
        {
            for (int i = 0; i<=5; i++)
            {
                if (i==0)
                {
                    Date d = new Date();
                    SimpleDateFormat ft = new SimpleDateFormat("hh:mm:ss");
                    System.out.println("Placing your order"
                            + " Item name "+ name +" = " +ft.format(d));

                }
                else
                {
                    Date d = new Date();
                    SimpleDateFormat ft = new SimpleDateFormat("hh:mm:ss");
                    System.out.println("Preparing - "+
                            name +" = " +ft.format(d));

                }
                Thread.sleep(1000);
            }
            System.out.println(name+" Prepared");
        }

        catch(InterruptedException e)
        {
            e.printStackTrace();
        }
    }
}
public class Tpi
{

    static final int MAX_T = 3;

    public static void main(String[] args)
    {

         Runnable r1,r2,r3;
         int price=0;
         ExecutorService pool = Executors.newFixedThreadPool(MAX_T);
        Scanner sc=new Scanner(System.in);
        int a[]=new int[100];
         int b[]=new int[100];
        int c[]=new int[100];
          int ch;
          int s=0;
          int n=0;
          int d=0;

          String[] main_dish={"dosa","Poori","pizza","Noodles","Biriyani","Fried rice","Parotta","Chilli parotta","Butter naan","tandoori","Mumbai_thaali","Rava_Bath","Spagatti","Chappathi","pulaav"};
          int[] mdprice={10,7,130,80,130,90,15,120,50,180,130,40,40,20,75};
          String[] Drinks={"apple","orange","Mango milkshake","Strawberry Milkshake","Chocolaate Milkshake","Black_Current","Lime_soda","Coke","Pepsi","7up","Jigarthanda","Mojito","Shaarjha","Lassi","Mountain_dew"};
          int[] driprice={20,20,30,30,30,35,25,30,35,30,25,40,35,35,30};
          String[] Soup={"Mushroom","Sweetcorn","Pepper","Vegetable_soup","Mutton_soup","Chicken_soup","Tomato_soup","Chicken_noodle_soup","Creamy_potato_soup","Brocolli_soup","Mexican_chilli_soup"};
          int[] souppri={120,110,100,125,150,140,90,90,70,50,80};
          String[] gravy={"paneer masala","Mushroon masala","Pepper chicken"};

          System.out.println("\n+-+-+--+-+-+-+-+-+-+-+NKS RESTAURENT+-+-+-+-+-+-+-+-+-+-+-+-+-+\n");
        System.out.println("A TASTE YOU'LL REMEMBER!!WHERE EVERY FLAVOUR TELLS A STORY!!");

          System.out.println("\n***************************\n           Menu\n***************************");
        System.out.println("\n1.SOUP\n2.MAIN DISH\n3.DRINKS\n4.BILL\n5.MAY BE LATER\n");

        do{
            System.out.println("Enter the choice");
        ch=sc.nextInt();
        if(ch==2){
        System.out.println("\n************************MAIN DISH******************************");
        System.out.println("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
        System.out.println("\tDISH NAME\t\t\tPRICE");
        System.out.println("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
        System.out.println("\t1.DOSA\t\t\t\t10\n\t2.POORI\t\t\t\t7\n\t3.Pizza\t\t\t\t130\n\t4.Noodles\t\t\t80\n\t5.Biriyani\t\t\t130");
        System.out.println("\t6.Fried rice\t\t\t90\n\t7.Parotta\t\t\t15\n\t8.Chilli parotta\t\t120\n\t9.Butter naan\t\t\t50\n\t10.Tandoori\t\t\t180");
        System.out.println("\t11.Mumbai thaali\t\t130\n\t12.Rava bath\t\t\t40\n\t13.Spagatti\t\t\t40\n\t14.chappathi\t\t\t20\n\t15.Pulaav\t\t\t75");
        System.out.println("\n***************************************************************");
        System.out.println("\nEnter the number of Main dishes you want:");
        s=sc.nextInt();
        System.out.println("\nEnter the dish number that you want to place an order:");
        for (int i = 0; i < s; i++) {
         if(s<5)
           {
             int k=sc.nextInt();
             a[i]=k-1;
             r1 = new Task(main_dish[k-1]);

            pool.execute(r1);
           }
           else
           {
               if(i!=s-1){
               int k=sc.nextInt();
               a[i]=k-1;
             r1 = new Task(main_dish[k-1]);

            pool.execute(r1);
               }
               if(i==s-1)
            {
                System.out.println("SORRY FOR THE INCONVINIENCE....Your order will reach you soon......Please wait");
            }
           }
        }

        }
        else if(ch==3)
        {
        System.out.println("\n****************************\nDrinks\n******************************\n");

        System.out.println("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
        System.out.println("\tDRINKS NAME\t\t\tPRICE");
        System.out.println("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");

        System.out.println("\n      1.Apple\t\t\t\t20\n      2.Orange\t\t\t\t20\n      3.Mango Mikshake\t\t\t30\n      4.Strawberry Milshake\t\t30\n      5.Chocolate Milkshake\t\t30");
             System.out.println("      6.Black currant Milkshake\t\t35\n      7.Lime soda\t\t\t25\n      8.Coke\t\t\t\t30\n      9.Pepsi\t\t\t\t35\n      10.7up\t\t\t\t30");
             System.out.println("      11.Jigarthanda\t\t\t25\n      12.Mojito\t\t\t\t40\n      13.Shaarjha\t\t\t35\n      14.Lassi\t\t\t\t35\n      15.Mountain_Dew\t\t\t30");
             System.out.println("\n***************************************************************");
             System.out.println("\nEnter the no. of Drinks you want:");
             n=sc.nextInt();
         System.out.println("\nEnter the Drink no :");

      for (int i = 0; i < n; i++) {
if(n<5)
           {
             int k=sc.nextInt();
             b[i]=k-1;
             r2 = new Task(Drinks[k-1]);


            pool.execute(r2);
           }
           else
           {
               if(i!=n-1){
               int k=sc.nextInt();
               b[i]=k-1;
             r2 = new Task(Drinks[k-1]);

            pool.execute(r2);
               }
               if(i==n-1)
            {
                System.out.println("SORRY FOR THE INCONVINIENCE....Your order will reach you soon....PLease wait");
            }
           }

        }
        }
        else if(ch==1)
        {
        System.out.println("\n************************************\n       Soup\n************************************");
         System.out.println("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
        System.out.println("\tSOUP NAME\t\t\tPRICE");
        System.out.println("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
 System.out.println("\n\t1.Mushroom Soup\t\t\t\t120\n\t2.Sweetcorn soup\t\t\t110\n\t3.Pepper soup\t\t\t\t100\n\t4.Vegetable soup\t\t\t125\n\t5.Mutton soup\t\t\t\t150\n\t6.Chicken soup\t\t\t\t140");
  System.out.println("\t7.Tomato soup\t\t\t\t60\n\t8.Chicken noodle soup\t\t\t90\n\t9.Creamy potato soup\t\t\t70\n\t10.Brocolli soup\t\t\t50\n\t11.Mexican chilli soup\t\t\t80\n");
  System.out.println("\nEnter the no. of Soup you want:");
         d=sc.nextInt();
         System.out.println("\nEnter the Starter's number:");
       for (int i = 0; i < d; i++) {
if(d<5)
           {
             int k=sc.nextInt();
             c[i]=k-1;
             r3 = new Task(Soup[k-1]);

            pool.execute(r3);
           }
           else
           {
               if(i!=d-1){
               int k=sc.nextInt();
               c[i]=k-1;
             r3= new Task(Soup[k-1]);
             c[i]=k-1;

            pool.execute(r3);
               }
               if(i==d-1)
            {
                System.out.println("SORRY FOR THE INCONVINIENCE........Your order will reach you soon...........PLease wait");

            }
           }
        }


        }
        else if(ch==4)
        {
        bill(main_dish,mdprice,a,s,Drinks,driprice,b,n,Soup,souppri,c,d);
        }


        }while(ch!=5);
        System.out.println("+-+-+-+-+-+-+-Bye bye!!!We are always here to serve you!!!!-+-+-+-+-+-+-+-+-+");



        pool.shutdown();
        }
public static void bill(String main_dish[],int mdprice[],int a[],int s,String Drinks[],int driprice[],int b[],int n,String Soup[],int souppri[],int c[],int d)
{
    int i,price=0;
    System.out.println("**********************************************************************************\n");
    System.out.println("                             NKS Restaurant                                         ");
    System.out.println("**********************************************************************************\n");
    System.out.println("                                  BILL                                             \n");
    for(i=0;i<s;i++)
    {
        System.out.println(main_dish[a[i]] +"-"+mdprice[a[i]]);                         price=price+mdprice[a[i]];
    }
    for(i=0;i<s;i++)
    {
        System.out.println(Drinks[b[i]] +"-"+driprice[b[i]]);

        price=price+mdprice[a[i]];
    }
    for(i=0;i<d;i++)
    {
        System.out.println(Soup[c[i]] +"-"+souppri[c[i]]);

        price=price+souppri[c[i]];
    }
    System.out.println("Total amount you want to pay\t\t"+price);
    System.out.println("\n+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+\n");
    System.out.println("                              Thank you!!Visit again                                      ");
}
}



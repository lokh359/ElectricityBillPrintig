# ElectricityBillPrintig
As we know that now-a-days printing become common at every point so i have decided to write the code for print the electrcity bill by using the java.
package com.company;
import org.w3c.dom.ls.LSOutput;

import java.util.Scanner;

public class ElectricityBill {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter the name of the Customer name:");
        String name=sc.nextLine();
        System.out.println("Enter the units of bill:");
        int unit=sc.nextInt();

        double bill;
        if(unit<=100)
        {
            System.out.println("********************************************");
            bill=unit*2;
            System.out.println("Name :"+name);
            System.out.println("Total Units consumed :"+unit);

            System.out.println("Total Bill :"+bill);
            System.out.println("********************************************");
        }
        else if (unit>=100 && unit<=200)
        {
            System.out.println("********************************************");
            System.out.println("Name :"+name);
            System.out.println("Total Units consumed :"+unit);
            bill=unit*3;
            System.out.println("Total Bill :"+bill);
            System.out.println("********************************************");
        }
        else if(unit>=200 && unit <=400)
        {
            System.out.println("********************************************");
            System.out.println("Name :"+name);
            System.out.println("Total Units consumed:  " +unit);
            bill=unit*4;
            System.out.println("Total Bill :"+bill);
            System.out.println("********************************************");
        }
        else
        {
            System.out.println("Report to the Current bill department");
        }


    }
}

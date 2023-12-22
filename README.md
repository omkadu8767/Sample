#Pract2 Pattern

import java.util.*;
class Pract2{
    public static void print(int n) {
        
        for(int i=0;i<=n;i++){
            for(int j=1;j<=i;j++ ){
                System.out.print(j+" ");
            }
            System.out.println();
        }
    }
    public static void main(String[] args) {
        int n=5;
        print(n);
    }
} 

#Pract3 Types Of Variable

import java.util.*;
public class Pract3 {
    int a=1;
    static int b=2;
    public static void main(String[] args) {
        int c=3;
        Pract3 obj=new Pract3();
        System.out.println(c+ ",is local variable");
        System.out.println(obj.a+",is instance variable");
        System.out.println(Pract3.b+", is static variable");
     }
}

#Pract4    Overloading

import java.util.Scanner;

public class Pract4 {
    int r, l, b;

    void area(int radius) {
        float a;
        r = radius;
        a = (float) 3.14 * r * r;
        System.out.println("Area of Circe=" + a);
    }

    void area(int length, int breadth) {
        int a;
        l = length;
        b = breadth;
        a = l * b;
        System.out.println("Area of rectangle=" + a);
    }

    public static void main(String[] args) {
        Pract4 obj=new Pract4();
        obj.area(5,9);
        obj.area(2);
    }
}

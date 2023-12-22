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

#Pract5 Sorting
public class Pract5 {
    public static void main(String[] args) {
        int arr[] = { 25, 40, 19, 8, 24 };
        int temp = 0;

        System.out.println("UnSorted Array:");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }

        for (int i = 0; i < arr.length - 1; i++) {
            for (int j = 0; j < arr.length - i - 1; j++) {
                if (arr[j] > arr[j + 1]) {
                    temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }

#Pract6 overriding
public class Pract6 {
    class Parent {
        void show() {
            System.out.println("Parent Class");
        }
    }

    class Child extends Parent {
        void show() {
            System.out.println("Child Class");
        }
    }

    public static void main(String[] args) {
        Pract6 pract6 = new Pract6(); 
        Child c = pract6.new Child(); 
        c.show();

        Parent p = pract6.new Parent(); 
        p.show();
    }
}

        System.out.println("\nSorted Array:");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}

#Pract7 multiple inheritance
public class Pract7 {
    interface Printable {
        void print();
    }

    interface Showable {
        void show();
    }

    class A implements Printable, Showable {
        public void print() {
            System.out.println("Hello");
        }

        public void show() {
            System.out.println("World");
        }
    }

    public static void main(String[] args) {
        A a = new Pract7().new A(); 
        a.print();
        a.show();
    }
}

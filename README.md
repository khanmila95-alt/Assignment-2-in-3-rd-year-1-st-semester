# Assignment-2-in-3-rd-year-1-st-semester

class Student {
       int age;

    void display() {
               int marks = 85;

        System.out.println("Instance Variable (age): " + age);
        System.out.println("Local Variable (marks): " + marks);
    }
}

public class StackHeapDemo {
    public static void main(String[] args) {
        // 's' (the reference) lives in the Stack
        // the Student object itself lives in the Heap
        Student s = new Student();
        s.age = 20;

        System.out.println("Student Object Created");
        System.out.println("Object Identity Hash Code: " + System.identityHashCode(s));

        s.display();
    }
}

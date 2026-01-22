public class Main {

    // Student class inside Main
    static class Student {
        // Private attributes
        private String name;
        private int age;
        private double grade;

        // Method nga naga set og student details
        public void setDetails(String n, int a, double g) {
            name = n;
            age = a;
            grade = g;
        }

        // Method nga para makuha ang student name
        public String getName() {
            return name;
        }

        // Method nga naga check kung naka passed ba ang student
        public boolean isPassed() {
            return grade >= 75;
        }

        // Method nga mo display sa information sa student
        public void displayInfo() {
            System.out.println("Student Name: " + name);
            System.out.println("Age: " + age);
            System.out.println("Grade: " + grade);

            if (isPassed()) {
                System.out.println("Status: Passed");
            } else {
                System.out.println("Status: Failed");
            }
        }
    }

    // Mao ni ang main method
    public static void main(String[] args) {
        
        Student student1 = new Student();

        
        student1.setDetails("Eroll John Llego", 20, 85.5);

        
        System.out.println("Student Name (from getName): " + student1.getName());
        System.out.println("Did the student pass? " + student1.isPassed());

        System.out.println("\n--- Student Information ---");
        student1.displayInfo();
    }
}

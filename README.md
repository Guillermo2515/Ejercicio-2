public class Programa3 {

    public static void main(String[] args) {
        System.out.println("Hello World!");
   
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese su edad: ");
        int edad = scanner.nextInt();

        if (edad >= 18) {
            System.out.println("Eres mayor de edad y puedes votar.");
        } else if (edad >= 16) {
            System.out.println("Eres menor de edad pero puedes votar.");
        } else {
            System.out.println("Eres menor de edad y no puedes votar.");
        }
    }
}

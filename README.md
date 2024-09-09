public class Ejercicio1 {

    public static void main(String[] args) {
        System.out.println("Bienvenido a la calculdora digital");
        Scanner scanner = new Scanner(System.in);
        short opcion;

        do {
            System.out.println("Menu de opciones");
            System.out.println("1. Sumar dos numeros");
            System.out.println("2. Restar dos numeros");
            System.out.println("3. Multiplicar dos numeros");
            System.out.println("4. Dividir dos numeros");
            System.out.println("5. Salir");
            System.out.print("Ingrese una opcion: ");
            opcion = scanner.nextShort();

            switch (opcion) {
                case 1 -> sumarDosNumeros(scanner);
                case 2 -> restarDosNumeros(scanner);
                case 3 -> multiplicarDosNumeros(scanner);
                case 4 -> dividirDosNumeros(scanner);
                case 5 -> System.out.println("Saliendo del programa");
                default -> System.out.println("Opcion invalida");
            }
        } while (opcion != 5);
    }

    private static void sumarDosNumeros(Scanner scanner) {
        System.out.print("Ingrese el primer numero: ");
        short num1 = scanner.nextShort();
        System.out.print("Ingrese el segundo numero: ");
        short num2 = scanner.nextShort();
        System.out.println("La suma es: " + (num1 + num2));
    }

    private static void restarDosNumeros(Scanner scanner) {
        System.out.print("Ingrese el primer numero: ");
        short num1 = scanner.nextShort();
        System.out.print("Ingrese el segundo numero: ");
        short num2 = scanner.nextShort();
        System.out.println("La resta es: " + (num1 - num2));
    }

    private static void multiplicarDosNumeros(Scanner scanner) {
        System.out.print("Ingrese el primer numero: ");
        short num1 = scanner.nextShort();
        System.out.print("Ingrese el segundo numero: ");
        short num2 = scanner.nextShort();
        System.out.println("La multiplicacion es: " + (num1 * num2));
    }

    private static void dividirDosNumeros(Scanner scanner) {
        System.out.print("Ingrese el primer numero: ");
        short num1 = scanner.nextShort();
        System.out.print("Ingrese el segundo numero: ");
        short num2 = scanner.nextShort();
        if (num2 != 0) {
            System.out.println("La division es: " + (num1 / num2));
        } else {
            System.out.println("Error: No se puede dividir por cero");
        }
    }
}

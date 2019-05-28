# Simpl-tasks-on-JAVA.-Task-3
 Напишите программу которая принимает 3 числовых значения и проверяет, могут ли они быть  *  сторонами треугольника.  *  Для ввода значений с консоли Вам понадобится класс Scanner.  *  &lt;code>Scanner scanner = new Scanner(System.in);&lt;/code>  *  &lt;code>scanner.nextInt();&lt;/code>


package controlstatement;

import java.util.Scanner;

public class task2 {
    public static void main(String[] args) {
        System.out.print("Введите параметры треугольника ");
        Scanner in = new Scanner(System.in);
        int a = in.nextInt();
        int b = in.nextInt();
        int c = in.nextInt();

        if ((a > b + c) || (b > a + c) || c > a + b) {
            System.out.println("Данные величины могут быть сторонами треугольника");
        } else {
            System.out.println("Введенные величины НЕ МОГУТ быть сторонам треугольника!");
        }

    }
}

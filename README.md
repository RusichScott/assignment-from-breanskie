
import java.util.Scanner;

   //создаём переменные для калькулятора 

public class Main {
   public static void main(String[] args) {
      double a;
      double b;
      double anser;
      Scanner src = new Scanner(System.in);
      System.out.print("Введите чила: ");
      a = src.nextDouble();
      b = src.nextDouble();
      System.out.print("Выберите метод (+, -, *, /): ");
      char op = src.next().charAt(0);
      solve(a,b,op);
   }
   
   //прописываем опирации нашего калькулятора 
   
   public static double solve(double a, double b, char op){
        double anser = 0;
        if (op == '+') {
            anser = a + b;
        }
        else if (op == '-') {
            anser = a - b;
        }
        else if (op == '*') {
            anser = a * b;
        }
        else if (op == '%') {
            anser = a % b;
        }
        else if (op == '/') {
        }
        System.out.println("Получай неуч - " + anser);
        return anser;
    }
}

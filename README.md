# JAVA-I
// Todos los TP resueltos de Java I
/*
 * UTN - Laboratio I - Trabajo Practico N`1
 * Autor: Matias Hector Martin
 * Ultima modificacion: Septiembre/2014
 */

package tp1;

/**
 *
 * @author matias
 */
import javax.swing.JOptionPane; //libreria para que muestre una ventana y meter datos del teclado
import java.util.Scanner;  //ESTA HERRAMIENTA PERMITE GRAVAR LO QUE SE ESCRIBE EN TECLADO 

public class TP1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        
        Scanner scan = new Scanner(System.in);

// EJERCICIO 1)
        
        System.out.println("EJERCICIO 1) Averiguar si un numero es divisible por otro.");
        
        String a;
        String b;
        
        a = JOptionPane.showInputDialog("Ingresa el primer numero");
        b = JOptionPane.showInputDialog("Ingrese el segundo numero"); 
        
        int conver_a = Integer.parseInt(a);// Para convertir variable de String a int(Entero)
        int conver_b = Integer.parseInt(b);
        
        if(conver_a % conver_b == 0 || conver_b % conver_a == 0)
            JOptionPane.showMessageDialog(null,"los numeros ingresados son divisibles entre si");
        else
            JOptionPane.showMessageDialog(null,"Los numeros ingresados NO son divisibles entre si");
        
// EJERCICIO 2)
        
        System.out.println("EJERCICIO 2) Tomando dos valores, devolver el numero mayor.");
        if (conver_a > conver_b)
            JOptionPane.showMessageDialog(null,"es mayor "+a+" que "+b);
        else
            JOptionPane.showMessageDialog(null,"es mayor "+b+" que "+a);
        
// EJERCICIO 3)
        
        System.out.println("EJERCICIO 3)");
        if(conver_a % 2 == 0)
            JOptionPane.showMessageDialog(null,"El primer numero ingresado ("+a+") es par");
        else
            JOptionPane.showMessageDialog(null,"El primer numero ingresado ("+a+") es impar");
        if(conver_b % 2 == 0)
            JOptionPane.showMessageDialog(null,"El segundo numero ingresado ("+b+") es par");
        else
            JOptionPane.showMessageDialog(null,"El segundo numero ingresado ("+b+") es impar");
            
              
// EJERCICIO 4)
        
        System.out.println("EJERCICIO 4)");    
        String cant_de_notas;
        int i, j, promedio, suma=0;
        
        cant_de_notas = JOptionPane.showInputDialog("Ingrese la cantidad de notas a promediar");
        int cant_notas = Integer.parseInt(cant_de_notas);
        cant_notas=scan.nextInt();
        
        for(i=1; i<=cant_notas; i++){
            JOptionPane.showInputDialog("Ingrese nota: "+i);
        j=scan.nextInt();    
        suma=suma+j;
        }
        promedio = suma / cant_notas;
        JOptionPane.showInputDialog("El promedio es: "+promedio);
        
//EJERCICIO 5)
       /* 
        String gripe = "fiebre";
        String miositis = "dolor_muscular";
        String sinusitis = "mucosidad";
        String dermatitis = "picazon";
        String sintoma;
        
        JOptionPane.showInputDialog("Ingrese su sintoma:");
        int grip = Integer.parseInt(fiebre);
        if(sintoma == fiebre)
            System.out.println("Posible enfermedad: "+);
        JOptionPane.showInternalConfirmDialog(null, scan, gripe, grip, grip)
      
        */
    }
    
}

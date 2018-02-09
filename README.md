# RecursividadFactorialJava

package calculofactorial;
public class CalculoFactorial {
 // declaración recursiva del método factorial
 public long factorial( long numero )
 {
 if ( numero <= 1 ) // evalúa el caso base
 return 1; // casos base: 0! = 1 y 1! = 1
 else // paso recursivo
 return numero * factorial( numero - 1 );
} // fin del método factorial

 // imprime factoriales para los valores del 0 al 10
 public void mostrarFactoriales()
 {
 // calcula los factoriales del 0 al 10
 for ( int contador = 0; contador <= 16; contador++ )
 System.out.printf( "%d! = %d\n", contador, factorial( contador ) );
 } // fin del método mostrarFactoriales
 } // fin de la clase CalculoFactorial




Metodo 

package calculofactorial;


public class PruebaFactorial {
    

// calcula los factoriales del 0 al 10
 public static void main( String args[] )
 {
 CalculoFactorial calculoFactorial = new CalculoFactorial();
 calculoFactorial.mostrarFactoriales();
 } // fin del método main
 } // fin de la clase PruebaFactorial



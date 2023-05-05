# Enumerados

Los tipos enumerados en Java permiten definir un conjunto de constantes con nombre, lo que facilita la lectura y el mantenimiento del código.

1. Ejemplo básico:
```
enum DiaSemana {
  LUNES, MARTES, MIERCOLES, JUEVES, VIERNES, SABADO, DOMINGO
}

public class EjemploEnum {
  public static void main(String[] args) {
    DiaSemana hoy = DiaSemana.MARTES;
    System.out.println("Hoy es " + hoy);
  }
}
```
Este ejemplo define un tipo enumerado `DiaSemana` que contiene los días de la semana. Se crea una variable `hoy` de tipo `DiaSemana` y se le asigna el valor `MARTES`. Luego se imprime el valor de `hoy` en la consola.

2. Ejemplo con constructor y método:
```
enum Color {
  ROJO(255, 0, 0),
  VERDE(0, 255, 0),
  AZUL(0, 0, 255);

  private int r, g, b;

  Color(int r, int g, int b) {
    this.r = r;
    this.g = g;
    this.b = b;
  }

  public String getRGB() {
    return "(" + r + ", " + g + ", " + b + ")";
  }
}

public class EjemploEnum {
  public static void main(String[] args) {
    Color miColor = Color.ROJO;
    System.out.println("Mi color es " + miColor.getRGB());
  }
}
```
En este ejemplo se define un tipo enumerado `Color` que tiene tres constantes: `ROJO`, `VERDE` y `AZUL`. Cada una de ellas tiene un constructor que recibe los valores de los componentes RGB y los asigna a las variables `r`, `g` y `b`. Además, se define un método `getRGB()` que devuelve una cadena con los valores de los componentes RGB de cada color. En el método principal se crea una variable `miColor` de tipo `Color` y se le asigna el valor `ROJO`. Luego se imprime el valor de `miColor.getRGB()` en la consola.




  

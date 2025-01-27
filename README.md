// exemplo da questão 1
abstract class Forma {
    abstract double calcularArea(); // Método abstrato
}

class Retangulo extends Forma {
    private double largura, altura;

    Retangulo(double largura, double altura) {
        this.largura = largura;
        this.altura = altura;
    }

    @Override
    double calcularArea() {
        return largura * altura;
    }
}

class Circulo extends Forma {
    private double raio;

    Circulo(double raio) {
        this.raio = raio;
    }

    @Override
    double calcularArea() {
        return Math.PI * raio * raio;
    }
}

public class TesteClassesAbstratas {
    public static void main(String[] args) {
        Forma forma = new Retangulo(5, 10);
        System.out.println("Área do Retângulo: " + forma.calcularArea());

        forma = new Circulo(7);
        System.out.println("Área do Círculo: " + forma.calcularArea());
    }
}

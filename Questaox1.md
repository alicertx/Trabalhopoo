// Exemplo de Polimorfismo
//questao 1 exemplo 
abstract class Animal {
    abstract void emitirSom(); 
}

class Cachorro extends Animal {
    @Override
    void emitirSom() {
        System.out.println("Au Au!");
    }
}

class Gato extends Animal {
    @Override
    void emitirSom() {
        System.out.println("Miau!");
    }
}

public class TestePolimorfismo {
    public static void main(String[] args) {
        Animal meuAnimal = new Cachorro(); // Polimorfismo
        meuAnimal.emitirSom(); // Saída: Au Au!

        meuAnimal = new Gato(); 
        meuAnimal.emitirSom(); 
    }
}

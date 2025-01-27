//exemplo da questao 4

interface Veiculo {
    void acelerar();
    void frear();
}

class Carro implements Veiculo {
    @Override
    public void acelerar() {
        System.out.println("Carro acelerando...");
    }

    @Override
    public void frear() {
        System.out.println("Carro freando...");
    }
}

class Moto implements Veiculo {
    @Override
    public void acelerar() {
        System.out.println("Moto acelerando...");
    }

    @Override
    public void frear() {
        System.out.println("Moto freando...");
    }
}

public class TesteInterface {
    public static void main(String[] args) {
        Veiculo veiculo = new Carro();
        veiculo.acelerar();
        veiculo.frear();

        veiculo = new Moto();
        veiculo.acelerar();
        veiculo.frear();
    }
}

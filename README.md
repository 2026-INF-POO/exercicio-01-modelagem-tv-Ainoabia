# Exercício: Modelagem TV

1. Edite o arquivo `TV.java` e construa uma modelagem para representar uma TV utilizando as informações abaixo. 

    Uma televisão possui as seguintes características:
    - tamanho de tela (em polegadas);
    - volume: de 1 a 10 iniciando em 5;
    - marca;
    - voltagem (220 e 110);
    - canal.

    A televisão pode realizar as seguintes ações:
    - ligar: ao ligar a televisão deve imprimir seu consumo. O consumo deve ser definido pela voltagem multiplicada pela quantidades de polegadas;
    - desligar;
    - aumentar e diminuir o volume;
    - subir e descer canal.

class TV {

    int tamanhotela;
    int volume = 5;
    String marca;
    int voltagem;
    int canal;
    int consumo;

    void ligar() {
        consumo = tamanhotela * voltagem;
        System.out.println("O valor do consumo é: " + consumo);
    }

    void desligar() {

    }

    void aumentarvol() {
        if (volume < 10) {
            volume++;
        }
    }

    void diminuirvol() {
        if (volume > 1) {
            volume--;
        }
    }

    void canalmais() {
        canal++;
    }

    void canalmenos() {
        canal--;
    }
}

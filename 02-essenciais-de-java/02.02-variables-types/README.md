# Variáveis e seus tipos

Em java suas variaveis são fortemente tipadas, sendo necessário ser definido seus tipos, não sendo possivel usar outro tipo em uma variavel com determinado tipo de variavel, são dois principais tipos aparesentados, os primitivos e os não primitivos.

# Primitivos

Os tipos primitivos tem um valor padrão de inicialização, ocupando um espaço específico em memória.

- Numeric
  - character
    - char
  - integral
    - integer
      - byte
      - short
      - int
      - long
    - floating-point
      - float
      - double
- boolean
  - boolean

| Tipo Primitivo | Valor padrão de inicialização | Tamanho |	Limite de armazenamento |
| :--: | :--: | :--: | :-- |
| byte | 0 | 1 byte | -128 até 127 |
| short | 0 | 2 byte |	-32,768 até 32,767 |
| int | 0 | 4 byte | -2,147,483,648 até 2,147,483, 647 |
| long | 0L | 8 byte | -9,223,372,036,854,775,808 até 9,223,372,036,854,775,807 |
| float | 0.0f | 4 byte | -1.4E-45 até 3.4028235E38 |
| double | 0.0d | 8 byte | -4.9E-324 até 1.7976931348623157E308 |
| char | '\u0000' | 2 byte | 0 até 65535 |
| boolean | false | 1 bit |true ou false |

Muito usados para armazenamento de valores temporários e execução de algoritmos. Para garantir que o os algoritmos criados tenha uma alta performance foi definido essas limitações núméricas.

O `byte` é o tipo de menor unidade para armazenamento dos inteiros, considerando que 1 byte é composto por 8 bits.

```
public class TiposPrimitivos {

    public static void main(String[] args) {
        byte b = 9;
        System.out.println(b);  
    }
}
```

O `short` tem um range maior(conforme a tabela) e são usados quando é criado algum algoritmo com uma interação de valores numéricos não muito grandes.

```
public class TiposPrimitivos {

    public static void main(String[] args) {
        short num = 300;
        short formatadaComUnderscore = 20_000; // variável 
        System.out.println(num);
        System.out.println(formatadaComUnderscore); // 20000
    }
}
```

Números podem conter símbolos `_` (underscore) para facilitar a leitura. (1_000_000).

O `int` possui um range conforme a tabela, sendo tipos inteiros usados para resolver problemas com algoritmos simples.

```
public class TiposPrimitivos {

    public static void main(String[] args) {
        int numeroInteiro = 10;
        int a = 10, b = 20, soma; // inicialização de variáveis inline
        soma = a + b; // atribuição da soma da variável a + b para a variável soma
        System.out.println(numeroInteiro); // 10
        System.out.println(soma); // 30
    }
}
```

O `long` tem um range conforme a tabela, sendo o tip que armazena a maior quantidade de números inteiros.

```
public class TiposPrimitivos {

    public static void main(String[] args) {
        long numA = 102040;
        long numB = 102030405060L; // adicionado L no final para indicar que estamos inserindo um valor do tipo long
        System.out.println(numA);
        System.out.println(numB);
    }
}
```

Usando o L ao final do valor, indica ao java que está sendo usado um número grande, deixando mais explicito.

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


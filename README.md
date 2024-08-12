Integrantes
Carlos Reis – RA: 2401937
Natalia Reis – RA: 2401504
Luigi Lago – RA: 2400428
Gabriel Padula – RA: 2402305
Julio Dyna – RA: 2402440

Trabalho do MBA de Data science e Advanced Analytics

Materia: Data science com Python
Professora: Carolina Zambelli
08/2024


Definição das funções e entradas e saidas

Ao executar o arquivo “decode_morse.py” o terminal irá solicitar a entrada de uma frase qualquer, desde que não contenha caracteres especiais, letras com acentos e cedilha, com cada palavra separada por espaço simples, como a escrita normal e sem pontuação, podendo ser letras e números inteiros (não negativos).
Como saída é gerado um arquivo CSV salvo na mesma pasta do projeto, que contém 3 colunas: na primeira coluna a frase inserida, na segunda o timestamp (data e hora) da criação da frase e na última o código desta frase em Morse. 
As funções estão em um arquivo chamado “decode_morse.py”, estão separadas de forma que seja possível importar essas funções em outros projetos e códigos, e o dicionário para código morse está no arquivo “config.py”.
As funções são: 

invert_dict(reverso) - Esta função recebe como argumento o dicionário, referenciado na variável “reverso” e o inverte. Aquilo que era chave se torna valor e vice versa. O retorno é o dicionário invertido. Usado para reverter o dicionário para morse, assim seria possível converter de alfa numérico para morse. 

adicionar_espaco_entre_letras(palavra) - Esta função recebe uma palavra ou frase e adiciona o caractere espaço entre as letras. O retorno é a palavra ou frase com um caractere espaço entre cada letra e o caractere “pipe” ( | ) onde antes havia um espaço normal.

code_morse_create(msg) - Esta função recebe como input a palavra ou frase que se deseja converter em código morse, a palavra ou frase pode ser escrita normalmente, respeitando o indicado como input pelo teclado (que não contenha caracteres especiais, letras com acentos e cedilha, com cada palavra separada por espaço simples, como a escrita normal e sem pontuação, podendo ser letras e números inteiros (não negativos)). A Saída é a palavra ou frase codificada em código morse. 

decode_morse(msg) - Esta função recebe a mensagem codificada em código morse. Sua saída é a mensagem decodificada. 

save_clear_msg_csv_hdr(msg) - Esta função recebe a mensagem codificada em código morse. Sua saída é gravada em um arquivo CSV, onde terão 3 colunas: a primeira coluna a frase inserida, na segunda o timestamp (data e hora) da criação da frase e na última o código desta frase em Morse.

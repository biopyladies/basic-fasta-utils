# Basic-Fasta-Utils

Este repositório faz parte do miniprojeto proposto para as Pyladies Bioinfo do Nível Básico. Contém funções Python para manipulação de arquivos FASTA contendo sequências de proteínas. As principais funcionalidades são a leitura de arquivos FASTA e a obtenção de propriedades biológicas sobre as sequências.

## Funções

**`read_fasta(fasta)`**

Esta função lê um arquivo FASTA contendo sequências de proteínas e retorna um dicionário onde as chaves são os nomes das sequências e os valores são as próprias sequências.

Parâmetros:
- `fasta`: `str` - Caminho para o arquivo FASTA.

**`get_pop(dicio_fasta)`**

Esta função recebe um dicionário de sequências de proteínas (como o retornado por `read_fasta`) e calcula as propriedades biológicas para cada sequência.

Parâmetros:
- `dicio_fasta`: `dict`- Dicionário de sequências de proteínas.

Retorno:

Um dicionário onde as chaves são os nomes das sequências, e os valores são listas contendo o comprimento e o ponto isoelétrico.

## Exemplo de Uso

```python
# Leitura do arquivo FASTA
dicio_fasta = read_fasta('caminho/do/arquivo.fasta')

# Obtenção das propriedades das sequências
dicio_pop = get_pop(dicio_fasta)
```



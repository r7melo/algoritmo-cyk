# Implementação: Forma Normal de Chomsky e Algoritmo CYK

Este repositório contém a implementação do Trabalho Extra da disciplina de **Linguagens Formais e Autômatos** da **Universidade Federal do Ceará (UFC) - Campus de Crateús**.

## Sobre o Projeto

O objetivo deste projeto é aplicar conhecimentos sobre linguagens livres de contexto, implementando o processo completo de normalização de gramáticas e reconhecimento de palavras.

O software foi desenvolvido para realizar a transformação de uma **Gramática Livre de Contexto (GLC)** qualquer para a **Forma Normal de Chomsky (FNC)** e, posteriormente, utilizar o algoritmo **Cocke-Younger-Kasami (CYK)** para verificação de pertinência de palavras.

## Funcionalidades

De acordo com as especificações do trabalho, o programa realiza as seguintes operações:

* **Entrada de Dados:** Recebe uma GLC $G=(V,T,P,S)$ e uma palavra $w$.
* **Normalização:** Realiza a transformação da gramática $G$ fornecida para sua equivalente na Forma Normal de Chomsky (FNC).
* **Algoritmo CYK:** Aplica o algoritmo de Cocke-Younger-Kasami (uma abordagem de Programação Dinâmica *bottom-up*) para determinar se a palavra $w$ pertence à linguagem gerada pela gramática.
    * *Nota:* O algoritmo possui tempo de processamento proporcional a $|w|^3$.

# Configurações

## Ambiente Virtual
Para criação do ambiente virtual, execute:
```
python -m venv venv
```
Para ativar o ambiente e começar a desenvolver, execute:
1. Windows: 
    ```
    venv\Scripts\activate
    ```
1. Linux/macOS:
    ```
    source venv/bin/activate
    ```
Após o ambiente ativado, execute o comando abaixo para instalção das dependências:
```bash
pip install -r .\requirements.txt
```
Com as dependências instaladas, incie o jupyter notebook, executando:
```
jupyter notebook
```
Logo, será aberto uma aba no navegador com o projeto, e dentro da pasta **notebooks**, abrir o notebook principal.

## Estrutura do Projeto
O projeto se baseia na hierarquia de diretorios abaixo:
```
minimizacao-de-automato-finito/
│
├─ notebooks/        # Notebooks Jupyter
├─ docs/             # Documentos Gerais
├─ src/              # Código Python reutilizável
├─ data/             # Dados de Entrada/Saída
│   ├─ raw/          # Dados originais (Entrada)
│   └─ processed/    # Dados processados (Saída)
├─ requirements.txt  # Dependências do projeto
└─ README.md         # Documentação de apresentação
```




# Referencias
- Livro: Linguagens Formais e Autômatos Nº3, Paulo Blauth Menezes
- [Linguagens Formais e Autômatos, MVM Ramos - 2008](https://www.marcusramos.com.br/univasf/lfa-2008-1/Apostila.pdf)
- [EducationAboutStuff - YouTube](https://www.youtube.com/watch?v=VTH1k-xiswM)

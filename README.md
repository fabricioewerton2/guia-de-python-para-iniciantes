# 🐍 Guia de Python para Iniciantes 🐍

Este repositório é um guia de estudos estruturado para aprender Python Básico. Ele reúne uma curadoria de materiais de referência, métodos de estudo práticos e o uso de Engenharia de Prompts para acelerar e consolidar o aprendizado.

---

## 🎯 1. Contexto e Objetivos

### Assunto de Interesse
O assunto escolhido para este caderno temático é a **Programação Básica com Python**. O guia vai desde a sintaxe elementar (variáveis, tipos básicos, operadores aritméticos/lógicos) e controle de fluxo (decisão e repetição), até conceitos de nível intermediário (modularização, tratamento de exceções, coleções dinâmicas e introdução à Programação Orientada a Objetos). O objetivo é formar uma base conceitual e prática robusta, essencial tanto para o desenvolvimento de software geral quanto para áreas correlatas como Ciência de Dados e Desenvolvimento Web.

### Objetivos de Estudo
*   **Domínio da Sintaxe e Semântica de Python:** Desenvolver a capacidade de escrever códigos limpos, legíveis e em conformidade com as diretrizes de estilo oficiais da linguagem (PEP 8).
*   **Pensamento Algorítmico e Resolução de Problemas (*Problem Solving*):** Ser capaz de decompor problemas complexos em funções modulares reutilizáveis e tratar erros em tempo de execução de forma elegante.
*   **Aceleração de Aprendizado com IA:** Documentar, compreender e estruturar a interação com modelos de linguagem, utilizando prompts estratégicos como aceleradores cognitivos na revisão e fixação de conceitos.

---

## 📚 2. Fontes utilizadas neste guia

Para garantir o rigor técnico e a qualidade didática deste caderno, selecionamos e indexamos as seguintes fontes de referência abertas e profissionais:

1.  **Curso Intensivo de Python (Eric Matthes - Novatec)** 
2.  **E-Book Python Básico (Marcos Roberto Ribeiro - IFMG, 2022)** 
3.  **Introdução ao Python (Google for Developers)** 
4.  **Python for Data Analysis, 3ª Edição (Wes McKinney)** 
5.  **Think Python: How to Think Like a Computer Scientist (Allen B. Downey)** 

---

## 🧠 3. Engenharia de Prompts & "Cicatrizes" de Troubleshooting

O desenvolvimento deste projeto de estudo envolveu o uso estratégico de Inteligência Artificial para gerar explicações personalizadas, diagramas de fluxo e resumos conceituais. Abaixo estão documentadas as interações estratégicas, as variações de prompts testadas e as "cicatrizes" de resolução de problemas encontradas durante a jornada.

### Perguntas Estratégicas & Variações de Prompts

A tabela abaixo registra o processo de refinamento de prompts para obter o melhor resultado didático:

| Prompt Inicial (Testado) | Comportamento da IA / Desafio | Prompt Otimizado (Aplicado) | Raciocínio de Engenharia |
| :--- | :--- | :--- | :--- |
| *"Me ensine a programar em Python baseado nos arquivos do meu notebook."* | A resposta foi excessivamente genérica, misturando conceitos avançados (como Programação Orientada a Objetos e APIs) logo no início, sem uma progressão pedagógica estruturada. | *"Crie um Guia de Estudos completo de Python em Markdown voltado para iniciantes, ideal para ser publicado em um arquivo README.md. Organize o guia com Visão Geral, Cronograma dividido por semanas (com checklists), Tópicos-Chave explicando conceitos em linguagem simples, Checkpoints de validação prática e Glossário técnico."* | **Clareza de Estrutura e Escopo:** Definir a persona (iniciante), o canal final (README.md no GitHub) e exigir a divisão por blocos lógicos estruturados força a IA a planejar o conteúdo sequencialmente de forma didática. |
| *"Explique as estruturas condicionais e de repetição em Python com código prático."* | O modelo gerou explicações corretas, mas poluiu o README com anotações de citações acadêmicas e colchetes numéricos (como `[1]`, `[12]`) que vieram da indexação da base de dados do NotebookLM. | *"Gere uma nova versão do README removendo todas as citações e notas de rodapé de colchetes numéricos (ex: `[...]`). Mantenha os colchetes dos checklists do GitHub (`- [ ]`) intactos."* | **Polimento de Formatação:** Para que um portfólio de projetos no GitHub passe credibilidade para recrutadores, ele deve estar limpo de marcadores de interface de ferramentas. A engenharia de prompts foi usada aqui para sanitizar o código e manter apenas a sintaxe nativa do Markdown do GitHub. |

### Cicatrizes de Troubleshooting (Resolução de Erros Práticos)

Abaixo estão os erros de depuração clássicos documentados durante os testes de código no console do interpretador interativo (`>>>`), que ajudaram a moldar o aprendizado prático:

1.  **O Erro de Indentação (`IndentationError: expected an indented block`):**
    *   *Sintoma:* O interpretador rejeitava a execução do laço `for` ou da condicional `if`.
    *   *Causa:* O Python não utiliza chaves `{}` para delimitar blocos de código; ele usa a indentação vertical (espaços em branco). Misturar tabulações com espaços em editores de texto causava conflitos de formatação.
    *   *Correção (Troubleshooting):* Configurar o editor de código (como Spyder ou VS Code) para substituir automaticamente a tecla TAB por 4 espaços consecutivos e garantir que todas as instruções internas do bloco estejam alinhadas horizontalmente à direita.
2.  **O Erro de Nome Não Definido (`NameError: name 'mesage' is not defined`):**
    *   *Sintoma:* O programa finalizava repentinamente ao executar uma instrução print.
    *   *Causa:* Digitação incorreta do nome de uma variável que não havia sido previamente inicializada na memória.
    *   *Correção (Troubleshooting):* O "Traceback" (rastreamento de erros) do interpretador Python aponta exatamente a linha e o arquivo onde a inconsistência aconteceu. O erro foi solucionado corrigindo a ortografia de `mesage` para `message`.
3.  **O Erro de Concatenação de Tipos Mistos (`TypeError`):**
    *   *Sintoma:* Mensagem de erro ao tentar combinar mensagens textuais e resultados matemáticos: `TypeError: can only concatenate str (not "int") to str`.
    *   *Causa:* O Python é uma linguagem fortemente tipada e impede a junção direta de uma string (`str`) com um valor numérico (`int` ou `float`).
    *   *Correção (Troubleshooting):* Utilizar a função embutida `str()` para converter o valor numérico antes de concatenar (ex: `print("Resultado: " + str(numero))`) ou adotar as f-strings modernizadas (`print(f"Resultado: {numero}")`).

---

## 📖 4. Miniguia de Estudo

Esta seção apresenta o resultado consolidado e estruturado dos nossos estudos de Python. Utilize as caixas de seleção (`- [ ]`) no seu repositório para acompanhar seu progresso diário!

## 📅 Cronograma Semanal & Checklist de Progresso

Utilize os checklists abaixo para acompanhar sua evolução diária.

### Semana 1: Fundamentos, Variáveis e Operadores
- [ ] **Dia 1:** Configuração do ambiente (Interpretador Python, IDE Spyder ou editor de texto como Sublime Text/Geany).
- [ ] **Dia 2:** Executar seu primeiro `Hello World!` e entender variáveis (tipagem dinâmica e nomes permitidos).
- [ ] **Dia 3:** Manipulação de Strings (métodos `.upper()`, `.lower()`, `.title()`, `.strip()` e concatenação).
- [ ] **Dia 4:** Entrada e Saída de dados (`print()`, `input()`) e números (`int` e `float`).
- [ ] **Dia 5:** Expressões aritméticas, relacionais e lógicos. Uso da biblioteca `math` e funções embutidas.

### Semana 2: Controle de Fluxo (Decisões e Repetições)
- [ ] **Dia 6:** Estruturas de Decisão Simples e Compostas (`if` e `if-else`).
- [ ] **Dia 7:** Estruturas de Decisão Aninhadas e sintaxe `if-elif-else`.
- [ ] **Dia 8:** Laço de repetição `while` e o papel das flags (variáveis de controle do estado ativo).
- [ ] **Dia 9:** Laço de repetição `for` para percorrer sequências.
- [ ] **Dia 10:** Controle de repetição com instruções `break` e `continue`. Estilo PEP 8 de formatação.

### Semana 3: Modularização e Tratamento de Exceções
- [ ] **Dia 11:** O que são Exceções e como tratar erros de forma elegante com blocos `try-except`.
- [ ] **Dia 12:** Criação de funções personalizadas com `def`, parâmetros posicionais e nomeados.
- [ ] **Dia 13:** Funções com parâmetros opcionais (valores default) e retorno de valores com `return`.
- [ ] **Dia 14:** Conceito e uso prático de Recursão (função que chama a si mesma).
- [ ] **Dia 15:** Divisão de códigos em múltiplos arquivos: criação de módulos e importações (`import`, `from ... import`, aliases `as`).

### Semana 4: Coleções de Dados (Listas, Tuplas, Conjuntos e Dicionários)
- [ ] **Dia 16:** Listas em Python: estruturas dinâmicas, ordenação permanente (`sort()`), temporária (`sorted()`) e fatiamento.
- [ ] **Dia 17:** Matrizes (listas bidimensionais) e List Comprehensions.
- [ ] **Dia 18:** Tuplas: coleções imutáveis para proteção de dados fixos.
- [ ] **Dia 19:** Conjuntos (`set`): coleções não ordenadas sem elementos duplicados e suas operações matemáticas.
- [ ] **Dia 20:** Dicionários: mapeamento de chaves imutáveis para valores, iteração e aninhamento complexo.

### 🌟 Semana Extra (Aprofundamento): POO, Arquivos e Testes
- [ ] **Tópico 1:** Programação Orientada a Objetos: Classes, instanciação, parâmetros `self`, construtor `__init__()` e herança.
- [ ] **Tópico 2:** Manipulação de Arquivos de texto (`with open()`, métodos de leitura `read()`, `readlines()` e escrita `write()`).
- [ ] **Tópico 3:** Persistência de dados complexos: gravação e leitura de dados gerados pelo usuário com o módulo `json` (`json.dump` e `json.load`).
- [ ] **Tópico 4:** Testes de Unidade: testar funções e classes utilizando a biblioteca-padrão `unittest`.

---

## 📚 Tópicos-Chave Detalhados & Códigos de Exemplo

### 1. Fundamentos & Tipagem Dinâmica
Em Python, as variáveis não precisam ter seus tipos declarados explicitamente (tipagem dinâmica). O próprio interpretador descobre o tipo do dado no momento da atribuição.

```python
# Declarando tipos básicos
nome = "Guido" # str (texto)
idade = 35 # int (inteiro)
altura = 1.75 # float (ponto flutuante)
esta_ativo = True # bool (booleano)

# Verificando o tipo da variável em tempo de execução
print(type(nome)) # Saída: <class 'str'>
print(type(altura)) # Saída: <class 'float'>
```

#### Regras para Nomes de Variáveis:
* Podem conter apenas letras, números e underscores (`_`).
* Devem começar com uma letra ou underscore, nunca com números.
* Espaços não são permitidos; use underscores para separar palavras (ex: `meu_nome`).
* Evite usar palavras reservadas do Python (como `print`, `if`, `while`, etc.) como nomes.

---

### 2. Manipulação Avançada de Strings
Strings são sequências de caracteres de texto. Métodos importantes ajudam a formatar e limpar dados textuais recebidos do usuário (muito usado antes de salvar registros).

```python
mensagem = " aprendendo python é incrível! "

# Formatação de Letras
print(mensagem.upper()) # Letras maiúsculas
print(mensagem.lower()) # Letras minúsculas
print(mensagem.title()) # Primeira letra de cada palavra em maiúscula

# Limpeza de Espaços em Branco
print(mensagem.strip()) # Remove espaços do início e do fim
print(mensagem.lstrip()) # Remove espaços apenas da esquerda
print(mensagem.rstrip()) # Remove espaços apenas da direita

# Concatenação e Interpolação
nome_aluno = "Ana"
mensagem_pessoal = f"Olá, {nome_aluno.title()}, você gostaria de aprender Python hoje?"
print(mensagem_pessoal)
```

---

### 3. Operadores & Biblioteca `math`
Python possui uma gama de operadores aritméticos completos (incluindo divisões e potências de forma direta) e operadores relacionais/lógicos.

#### Operadores Aritméticos Práticos:
| Operador | Operação | Exemplo | Resultado |
| :---: | :---: | :---: | :---: |
| `+` | Adição | `5 + 3` | `8` |
| `-` | Subtração | `10 - 2` | `8` |
| `*` | Multiplicação | `4 * 2` | `8` |
| `/` | Divisão Real | `16 / 2` | `8.0` |
| `//` | Divisão Inteira (descarta decimal) | `17 // 2` | `8` |
| `%` | Resto da Divisão (módulo) | `17 % 2` | `1` |
| `**` | Exponenciação (Potência) | `2 ** 3` | `8` |

#### Biblioteca `math` (Exemplos Úteis):
```python
import math

print(math.ceil(4.2)) # Arredonda para cima (Teto) -> 5
print(math.floor(4.8)) # Arredonda para baixo (Piso) -> 4
print(math.sqrt(16)) # Raiz quadrada -> 4.0
print(math.pi) # Constante Pi -> 3.141592653589793
```

---

### 4. Estruturas de Decisão (`if-elif-else`)
Decidir quais partes do código executar com base em condições lógicas avaliadas como Verdadeiras (`True`) ou Falsas (`False`).

```python
# Simulação de alíquotas do imposto de renda simplificado
salario = 2500.00

if salario <= 1903.98:
 print("Isento de Imposto de Renda")
elif salario <= 2826.65:
 imposto = salario * 0.075
 print(f"Alíquota de 7.5%. Imposto a pagar: R$ {imposto:.2f}")
elif salario <= 3751.05:
 imposto = salario * 0.15
 print(f"Alíquota de 15%. Imposto a pagar: R$ {imposto:.2f}")
else:
 print("Alíquota superior")
```

---

### 5. Repetições Controladas (`while` & `for`)
* Use `for` quando souber previamente o número de repetições ou quando for iterar sobre coleções de dados (como listas).
* Use `while` quando a repetição depender de uma condição lógica cujo término não se sabe de antemão (ex: manter o programa rodando até o usuário decidir sair).

```python
# Exemplo de laço FOR gerando listas numéricas com range()
# range(start, stop, step) -> de 1 a 20 pulando de 2 em 2 (ímpares)
numeros_impares = list(range(1, 20, 2))
for numero in numeros_impares:
 print(f"Número ímpar: {numero}")

# Exemplo de laço WHILE com flag 'ativo' e parada break
ativo = True
while ativo:
 entrada = input("Digite algo (ou 'sair' para encerrar): ")
 if entrada.lower() == 'sair':
 ativo = False # Alternativa: usar a instrução break diretamente
 else:
 print(f"Você digitou: {entrada}")
```

---

### 6. Funções e Escopo de Variáveis
Funções são blocos de código nomeados criados para executar tarefas específicas que podem ser reutilizadas diversas vezes ao longo de um programa.

```python
# Função com parâmetro opcional (valor padrão/default)
def descrever_cidade(cidade, pais="Brasil"):
 """Exibe uma descrição simples de uma localidade."""
 return f"{cidade.title()} está localizada no(a) {pais.title()}."

# Diferentes formas de realizar a chamada
print(descrever_cidade("Belo Horizonte")) # Usa o país default ("Brasil")
print(descrever_cidade("Paris", "França")) # Sobrescreve com o argumento posicional
print(descrever_cidade(pais="Argentina", cidade="Buenos Aires")) # Argumentos nomeados (ordem livre)
```

---

### 7. Tratamento Elegante de Erros (Exceções)
Exceções são objetos Python especiais usados para administrar erros gerados durante a execução do programa. O uso do bloco `try-except` previne que o seu script falhe inesperadamente e exiba tracebacks confusos para o usuário final.

```python
# Função para garantir a entrada de um número inteiro válido
def input_int(mensagem):
 while True:
 try:
 # Tenta realizar a conversão direta da entrada do usuário
 valor = int(input(mensagem))
 return valor
 except ValueError:
 # Captura o erro caso o usuário digite letras ou caracteres inválidos
 print("Erro: Entrada inválida. Por favor, digite um número inteiro.")

idade = input_int("Digite sua idade: ")
print(f"Idade cadastrada com sucesso: {idade} anos!")
```

---

### 8. Coleções de Dados

| Coleção | Tipo | Descrição | Exemplo |
| :--- | :--- | :--- | :--- |
| **Lista** | Mutável | Sequência ordenada de elementos mutáveis. Permite duplicatas. | `['maçã', 'banana', 'maçã']` |
| **Tupla** | Imutável | Sequência ordenada imutável (não pode ser alterada após criada). | `('segunda', 'terça', 'quarta')` |
| **Conjunto** | Mutável | Coleção não ordenada de elementos uniques (ignora duplicatas automaticamente). | `{'azul', 'verde', 'vermelho'}` |
| **Dicionário** | Mutável | Par chave-valor onde as chaves devem ser imutáveis e únicas. | `{'id': 101, 'nome': 'Carlos'}` |

```python
# 1. LISTAS (Ordenando e Copiando corretamente)
frutas = ["maracujá", "morango", "banana"]
frutas.append("abacaxi") # Adiciona um elemento

# Copiando de forma segura usando fatiamento [:] (evita duplicar referências)
copia_frutas = frutas[:]

# 2. DICIONÁRIOS (Iterando com loops)
usuario = {'username': 'marcos_dev', 'status': 'ativo', 'nivel': 3}

# Iterando sobre chaves e valores simultaneamente
for chave, valor in usuario.items():
 print(f"Chave: {chave} -> Valor: {valor}")
```

---

## 🛠️ Desafios semanais

A cada fim de semana, você deverá realizar esses desafios propostos, afim de consolidar o que foi estudado.
obs: Recomendo só avançar para a próxima semana quando conseguir resolver os exercícios propostos e entender o que foi feito.

### Checkpoint 1 (Ao final da Semana 1)
* **Desafio Conversor de Tempo:** Escreva um programa que receba uma quantidade inteira de segundos inserida pelo usuário e converta esse número em Horas, Minutos e Segundos.
 * *Exemplo de Saída:* 3665 segundos = 1 hora, 1 minuto e 5 segundos.
* **Desafio Juros Simples:** Crie uma calculadora de juros simples que solicite ao usuário os valores de Capital ($C$), Taxa de Juros ($I$) e Tempo ($T$). O programa deve retornar o Juro Calculado ($J = \frac{C \times I \times T}{100}$).

### Checkpoint 2 (Ao final da Semana 2)
* **Desafio Calculadora de Fatorial:** Desenvolva um script que solicite ao usuário um número inteiro $n$ e calcule o seu fatorial ($n! = n \times (n - 1) \dots \times 2 \times 1$) utilizando uma estrutura de repetição.
* **Desafio Calculadora Interativa Dinâmica:** Simule uma calculadora contínua. Peça a operação desejada (soma, subtração, multiplicação, divisão ou sair). Execute a conta, mostre o resultado e peça a operação novamente, interrompendo o ciclo apenas quando o usuário selecionar explicitamente a opção 'sair'.

### Checkpoint 3 (Ao final da Semana 3)
* **Desafio Módulo Matemático Personalizado:** Crie um arquivo chamado `matemática_util.py` contendo funções para verificar se um ano é bissexto (`ano_bissexto(ano)`) e calcular a quantidade de dias que um mês de um ano específico possui (`dias_mes(ano, mes)`). Crie um segundo script que importe esse módulo e processe datas lidas do teclado.

### Checkpoint 4 (Ao final da Semana 4)
* **Desafio Analisador de Médias Dinâmicas:** Construa um programa que pergunte a distância e a velocidade média de vários trechos de uma viagem. Calcule a velocidade média ponderada total da viagem. Ao final, use listas ou tuplas para mostrar quais trechos específicos estiveram com velocidade acima da média geral calculada.
* **Desafio Contador de Frequência de Elementos:** Escreva uma função que leia uma lista de números inteiros e use um dicionário para sumarizar quantas vezes cada número único aparece na lista original.

---

## 📖 Glossário & Jargões Fundamentais

* **Problem Solving:** A capacidade geral de analisar problemas complexos, decompô-los em etapas lógicas menores e desenhar soluções sistêmicas eficientes através de algoritmos.
* **Sintaxe:** O conjunto de regras gramaticais e estruturais que definem como os blocos de códigos de um programa de computador devem ser escritos em uma determinada linguagem para serem considerados válidos.
* **Semântica:** O significado lógico ou o comportamento prático esperado das instruções válidas que compõem o programa. Um erro semântico ocorre quando o código roda sem quebras, mas produz um resultado incorreto.
* **Interpretador:** O software encarregado de ler o código escrito em uma linguagem de alto nível (como Python) e executá-lo passo a passo no processador, sem necessidade de uma compilação prévia de código executável.
* **Biblioteca-Padrão (Standard Library):** A coleção de módulos, funções e tipos integrados por padrão na distribuição do Python, sempre prontos para uso (como `math`, `json`, `collections` e `unittest`).
* **Docstring:** Strings especiais delimitadas por três aspas duplas (`"""`) colocadas logo no início de funções, classes ou módulos para documentar seu funcionamento de forma padronizada.
* **Aninhamento (Nesting):** O ato de embutir uma estrutura lógica dentro de outra do mesmo tipo (por exemplo, um dicionário dentro de uma lista, ou uma instrução condicional `if` dentro de outra).
* **Imutabilidade:** A propriedade de um tipo de dado que impede que seu valor interno seja alterado de forma direta após ser criado na memória (como strings, inteiros, floats e tuplas).
* **Instanciação:** O ato prático de criar um objeto individual único a partir do modelo geral estruturado e definido por uma Classe.
* **Exceção:** Um objeto especial gerado automaticamente quando ocorre algum erro lógico ou físico durante a execução de um programa, interrompendo sua execução caso não seja capturado.
* **Query:** Uma instrução de consulta estruturada enviada ao banco de dados para extrair ou manipular dados específicos que atendem a um conjunto de regras ou filtros definidos.

---

## 🔄 5. Prompts Reutilizáveis para Estudos e Revisões Futuras

Aqui estão alguns modelos de promps que você pode copiar e colar no seu assistente de IA para te apoiar em revisões, simular cenários de teste e aprofundar seu conhecimento sobre qualquer assunto deste guia:

### 🎯 1. O Prompt do "Simulado de Código" (Fixação de Checkpoints)
> *"Aja como um professor-tutor sênior de Python altamente didático. Crie 3 exercícios práticos progressivos (nível fácil, médio e desafiador) focados no assunto: **[Inserir Assunto, ex: Semana 2 - Laços de Repetição While e Flags]**. Apresente apenas os enunciados. Não me dê as soluções de imediato. Aguarde que eu envie os meus códigos de resposta para que você faça uma revisão técnica (Code Review), apontando erros de lógica, problemas de identação e sugerindo melhorias de estilo conforme a PEP 8."*

### 💡 2. O Prompt da "Metáfora Didática" (Explicação de Conceitos Abstratos)
> *"Explique o conceito de **[Inserir Conceito, ex: Programação Orientada a Objetos, Herança ou Dicionários]** em Python utilizando uma analogia simples e divertida do mundo real (como carros, receitas de bolo ou organização de gavetas). Evite jargões matemáticos complexos de imediato. Após a explicação da analogia, apresente um exemplo de código Python mínimo e comentado que ilustre essa metáfora prática."*

### 🛠️ 3. O Prompt de "Revisão e Refatoração de Código" (Refining)
> *"Analise o trecho de código Python abaixo com foco em boas práticas de engenharia de software. Identifique: 1) Possíveis bugs silenciosos (como loops infinitos ou tratamento ausente de erros); 2) Oportunidades de simplificação (usando list comprehensions ou funções embutidas); 3) Desvios de formatação em relação às regras da PEP 8. Forneça o código refatorado passo a passo, explicando o porquê de cada modificação.
> 
> **[Insira o seu código aqui]**"*

---

### 🎓 Como você pode contribuir e continuar estudando?
1. Faça um **fork** deste repositório para a sua conta do GitHub.
2. Clone o repositório localmente usando o Git (`git clone <url-do-repositorio>`).
3. À medida que completar os exercícios e checkpoints diários, altere o status das tarefas de `- [ ]` para `- [x]` no seu arquivo `README.md` e faça o commit das suas alterações (`git commit -am "Dia X concluído!"`).
4. Compartilhe o seu progresso na sua rede profissional para demonstrar a sua maturidade técnica e organização metodológica de estudos!

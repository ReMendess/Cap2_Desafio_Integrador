# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Cap 1 - Desafio Integrador: IA entre Robôs, Sinapses e Medicina

## Nome do grupo

# 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/in/renanmendes26/">Renan de Oliveira Mendes - RM563145</a>
- <a href="https://www.linkedin.com/in/ricaleone/">Ricardo Batah Leone - RM563382</a>
- <a href="https://www.linkedin.com/in/yuki-watanabe-kuramoto-858856146/">Yuki Watanabe Kuramoto  - RM565164</a>
- <a href="https://br.linkedin.com/in/rodrigoreinaux/">Rodrigo De Melo Reinaux Porto  - RM564242</a>


# 📜 Descrição
Nessa segunda fase desenvolvendo ferramentas que automatizam a triagem e o diagnóstico médico por meio de Processamento de Linguagem Natural (NLP) e Machine Learning. Utilizamos duas técnicas sw NLP, baseado em regras e estátistico.

Indo além, criamos uma interface moderna com React e Vite. Também desenvolvemos e treinamos um modelo de visão computacional para a análise de exames de eletrocardiograma.

# Links:

## Requisitos
#### Ambiente
Node.js 20.x ou 22.x LTS (recomendado para Vite 8) + npm
Python 3.10–3.12 
Portal web: Node 20/22, React 19, Vite 8, React Router 7. 
Notebook: Python 3.10–12, pip install -r requirements.txt (pandas, scikit-learn, numpy, JupyterLab).

#### Versões 
react ^19.2.4
react-dom ^19.2.4
react-router-dom ^7.13.2

pandas 2.1
scikit-learn 1.4
numpy 1.26
jupyterlab 4 



### Parte 1
Implementamos um sistema de extração de informações para interpretar relatos clínicos.

Através de buscas por palavras-chave e expressões comuns (ex: "aperto no tórax", "fadiga"), o algoritmo sugere diagnósticos preliminares como Infarto ou Insuficiência Cardíaca, simulando o apoio à decisão médica.

#### Como funciona:

 O sistema lê o arquivo de texto "sintomas_pacientes.txt" que tem descrições de sintomas e utiliza uma estrutura de mapeamento para identificar padrões semânticos.
 
 Como visto em aula, essa estratégia é baseada em regras, utilizando análises léxica, morfológica e sintática para compreender o texto.
 
<img src="assets/arquivo_txt.png" widht="150">

O código em python "Criar_Dados.py" cria uma base de dados simulado em CSV "mapa_sintomas_doencas.csv", seguindo uma estrutura onde o individuo apresenta até dois sintomas, intensidade, duração e uma doença passada na qual já foi diagnosticado.


<img src="assets/criar_dados.png" widht="150">

O programa "Identificar_sintomas.py" utiliza o arquivo .txt como base, cria uma ontologia com ele. Pega o arquivo csv e faz um mapeamento. Conforme encontra palavras e frases semelhantes, ele realiza um diagnóstico para paciente e registro dentro do arquivo csv.

<img src="assets/identificar_sintomas.png" widht="150">

Por fim criamos um programa "Visualizar_Ontologia" para visualizar a ontologia criada de forma visual e gráfica, permitindo entender a lógica de decisão do modelo de NLP baseado em regras.

<img src="assets/Mapa_Ontologia.png" widht="150">

### Parte 2


### Ir Além

### Ir Além 2

# 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>Dataset</b>: Nesta pasta está o arquivo .CSV escolhido, representando os dados númericos.

- <b>Imagens</b>: Aqui estão as 200 imagens de Raio-x do toráx e o programa "Cap1_Dados_Imagens_Selecao.ipynb" usado para selecionar essas imagens.

- <b>Textos</b>: Aqui estão os textos escolhidos para treinamento de um modelo NLP.
  
- <b>assets</b>: Imagens relevantes para documentação desse repositório.
  



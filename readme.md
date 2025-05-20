1. Explique com suas palavras o papel de cada camada da arquitetura MVC usada neste projeto.
Como o Model, o Controller e a View interagem entre si?

- Camada Model
    - Mantem-se os códigos responsáveis pela lógica do negócio
    - Armazenamento e recuperação de informações a partir de bancos de dados ou qualquer outro tipo de arquivo
    - Se comunica diretamente com o sistema de banco de dados
- Camada View
    - Mantem-se tudo que se refere à interface com o usuário
    - Arquivo HTML, CSS e JavaScript
- Camada Controller
    - Intermedeia a camada de dados (model) e a camada de apresentação (view)

2. Como ocorre o envio e o recebimento de dados no formato JSON neste projeto?
Cite uma rota que responde em JSON e explique seu funcionamento.

- O usuário acessa /alunos/curso/1 (por exemplo).
- O controller busca todos os alunos que pertencem ao curso com id = 1, usando o método Aluno.findByCurso(curso_id).
- Em vez de renderizar uma página HTML, a rota responde com os dados em formato JSON usando res.json(alunos).

3. Qual a importância de usar HTML básico com formulários e tabelas para organizar e manipular dados no navegador?
Por que esse tipo de estrutura ainda é útil em projetos back-end com Node.js?

Usar HTML básico com formulários e tabelas permite que o usuário envie e veja informações de forma simples. Formulários enviam dados para o servidor que são processados e armazenados, enquanto tabelas mostram listas organizadas, facilitando a visualização.

Vantagens do Node.js:
- Alta performance: Utiliza o motor V8 do Google Chrome, compilando JavaScript diretamente em código de máquina. 
- Escalabilidade: Capaz de lidar com um grande número de conexões simultâneas de maneira eficiente.
- Versatilidade: Permite o uso de JavaScript tanto no front-end quanto no back-end, facilitando o desenvolvimento full-stack.
- Grande ecossistema: Possui um vasto número de bibliotecas e frameworks disponíveis através do npm (Node Package Manager).
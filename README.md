🧾 Trabalho Prático – GitHub Actions

Aluno: Andreluc23
Disciplina: Frameworks e Ferramentas de Desenvolvimento
Tema: Integração de Workflows com GitHub Actions

🧩 1. Estrutura do Projeto

O projeto é composto por três arquivos principais:

Arquivo	Função
index.html	Página principal exibindo “Hello World” e a data/hora atual
style.css	Estilização da página (cores e fontes)
script.js	Código JavaScript que mostra a data/hora e realiza o cálculo 2+2 no console

Demonstração no navegador:
Ao abrir o arquivo index.html, é exibida a mensagem “Hello, World!” e a data/hora atual atualizadas automaticamente pelo script.js.

⚙️ 2. Automação com GitHub Actions

Foram criados cinco workflows dentro da pasta .github/workflows/, cada um com uma função específica.

🟩 1. push-utils.yml

Executa automaticamente a cada push no repositório.

Principais etapas:

Exibe “Hello, world!”

Mostra data e hora (UTC e horário de São Paulo)

Mostra o usuário responsável pelo push

Calcula e exibe 2 + 2 no terminal

Lista todos os arquivos do projeto

Conta arquivos .html

Cria automaticamente um README.md se ainda não existir

Alerta se houver arquivos maiores que 100KB

Gera relatório com os arquivos alterados

Verifica se o push contém arquivos .html, .css e .js

📸 Print sugerida: tela do workflow “Push Utilities” com o status Success e logs visíveis.

🌙 2. night-only.yml

Executa somente no período noturno (22h–05:59 no fuso de São Paulo).

📸 Print sugerida: log mostrando “Fora do período noturno. Encerrando.” ou “É noite. Prosseguir.”

📅 3. saturday-only.yml

Executa somente aos sábados, validando o dia da semana antes de rodar.

📸 Print sugerida: log com “É sábado. Prosseguir.” ou “Não é sábado. Encerrando.”

⏰ 4. nightly-count.yml

Executa automaticamente todos os dias à meia-noite (00:00 horário de São Paulo), contando a quantidade total de arquivos e exibindo o número de .html, .css e .js no repositório.

📸 Print sugerida: log com “00:00 SP → HTML: X CSS: Y JS: Z TOTAL: W”.

👋 5. hello.yml

Workflow de teste simples criado inicialmente para validar a execução do GitHub Actions.

✅ 3. Testes e Resultados

Todos os workflows foram executados com sucesso no GitHub Actions:

Workflow	Status	Resultado
hello.yml	✅ Success	Teste inicial de execução
push-utils.yml	✅ Success	Todos os passos concluídos
night-only.yml	✅ Success	Rodou conforme horário
saturday-only.yml	✅ Success	Validação de dia da semana
nightly-count.yml	✅ Success	Contagem de arquivos concluída

📸 Sugestão de print: tela igual à que você me mostrou, com todos os workflows verdes.

🧠 4. Conclusão

O projeto cumpre todos os requisitos propostos no enunciado:

Criação de repositório com HTML, CSS e JS.

Execução automática de workflows no GitHub Actions.

Validação de horários, datas, usuário e tamanho de arquivos.

Automatização de tarefas repetitivas com diferentes gatilhos (push e schedule).

O trabalho demonstra o uso prático do GitHub Actions como ferramenta de integração contínua (CI), com automações simples e eficazes aplicadas a um projeto real.

✍️ 5. Créditos

Desenvolvido por Andreluc23
Orientado pelo professor responsável pela disciplina.
Ano: 2025

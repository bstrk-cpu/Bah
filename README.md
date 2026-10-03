
📝 RedaçãoMaster | AI Essay Generator
Gerador de Redações Nota 1000 com Inteligência Artificial. Transforme qualquer tema em um texto dissertativo-argumentativo estruturado, coeso e com repertório sociocultural em segundos.

VersionLicenseTech StackAI

🚀 Funcionalidades
Geração Instantânea: Insira o tema e receba uma redação completa em menos de 30 segundos.
Estrutura ENEM: O texto segue rigorosamente a estrutura de 4 parágrafos (Introdução, 2 Desenvolvimentos e Conclusão).
Competência 5 Garantida: A conclusão sempre inclui a Proposta de Intervenção completa (Agente, Ação, Meio, Finalidade e Detalhamento).
Estilos de Escrita: Escolha entre tons diferentes:
Padrão ENEM: Formal e acadêmico.
Criativo: Foco em títulos impactantes.
Filosófico: Maior densidade de repertório literário/filosófico.
Sociológico: Foco em dados estatísticos e fatos sociais.
Ações Rápidas:
Copiar: Coloca o texto na sua área de transferência com um clique.
Baixar: Exporta a redação em arquivo .txt para estudo offline.
🛠️ Stack Tecnológica
Tecnologia	Descrição
HTML5	Estrutura semântica do site.
CSS3	Estilização moderna com Grid, Flexbox e variáveis CSS.
JavaScript (ES6+)	Lógica de interação, chamadas assíncronas à API e manipulação do DOM.
OpenAI API	Motor de geração de texto (GPT-4o).
📦 Instalação
O projeto é estático e não requer build tools (como Webpack ou Vite). Você pode abrir o arquivo index.html diretamente no navegador ou usar um servidor local.

1. Clonar o Repositório
bash
Download
Copy code
git clone https://github.com/seu-usuario/redacaomaster.git
cd redacaomaster
2. Configurar a API Key
O script chama a API da OpenAI diretamente do navegador. Para segurança, você pode manter a chave no código para uso local ou usar um Proxy (veja a seção de Segurança).

Edite o arquivo index.html e localize a variável:

javascript
Download
Copy code
const OPENAI_API_KEY = "sua_chave_api_aqui";
Substitua sua_chave_api_aqui pela sua chave real da OpenAI (começando com sk-...).

3. Rodar Localmente (Opcional)
Para uma experiência mais próxima da produção, use o servidor embutido do Python:

bash
Download
Copy code
python -m http.server 8000
Acesse http://localhost:8000 no seu navegador.

💻 Como Usar
Defina o Tema: Digite o tema proposto (ex: "O impacto das redes sociais na saúde mental de adolescentes").
Escolha o Estilo: Selecione o tom desejado no menu dropdown.
Adicione Repertório (Opcional): Se você já tem uma citação ou dado específico em mente, insira no campo "Referências Opcionais" para forçar a IA a usar.
Gerar: Clique em "Gerar Redação".
Revisar e Usar:
Leia o texto gerado na área de resultado.
Clique em "Copiar Texto" para colar no seu editor ou no sistema de avaliação online.
Ou clique em "Baixar .txt" para salvar.
⚙️ Como Funciona a IA (Prompt Engineering)
O coração do projeto é a função buildPrompt no JavaScript. Ela monta um prompt altamente estruturado para a IA. Aqui está um resumo da lógica:

text
Download
Copy code
1. Persona: "Atue como um redator especialista em vestibulares (Nota 1000)."
2. Estrutura Obrigatória:
   - Título: Máx 5 palavras, impactante.
   - Introdução: Contextualização + Tese (2 argumentos).
   - Desenvolvimento 1: Tópico frasal + Argumento + Repertório 1.
   - Desenvolvimento 2: Tópico frasal + Argumento + Repertório 2.
   - Conclusão: Retomada da tese + Proposta de Intervenção.
3. Restrições:
   - Tom formal/impessoal.
   - Conectivos variados.
   - Extensão: 25-30 linhas.
4. Saída: Apenas o texto limpo, sem explicações.
🔒 Segurança e Boas Práticas
Chave de API no Frontend: Para um projeto de demonstração, colocar a chave no JavaScript é aceitável, mas nunca faça isso em produção pública.
Solução: Use um Backend Proxy (Node.js, Python Flask, etc.) para receber a requisição do frontend e encaminhar para a OpenAI. Isso protege sua chave de vazamento.
Rate Limits: A API da OpenAI tem limites de requisições. O script não possui fila de espera nativa, mas a interface desabilita o botão durante a geração para evitar spam de cliques.
📂 Estrutura de Arquivos
Download
Copy code
redacaomaster/
├── index.html          # Página principal (HTML + CSS + JS)
├── README.md           # Este arquivo
└── .gitignore          # Arquivos ignorados pelo Git
🤝 Contribuindo
Contribuições são bem-vindas! Para sugerir melhorias:

Faça um fork do repositório.
Crie uma branch (git checkout -b feature/MinhaMelhoria).
Faça o commit (git commit -m 'Adiciona funcionalidade X').
Faça o push para a branch.
Abra um Pull Request.
Ideias de melhorias futuras:

 Salvar histórico de redações no localStorage.
 Sistema de avaliação automática (a IA nota a própria redação).
 Exportação para PDF formatado.
 Suporte a outros idiomas (Espanhol/Inglês).
📄 Licença
Distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

✍️ Autor
The b stark -
"A redação não é uma loteria, é um projeto de texto."

Copy message
Scroll to bottom

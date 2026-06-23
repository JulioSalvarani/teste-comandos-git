1. Configuração e Inicialização
  git init: Inicializa um novo repositório Git em uma pasta local 
  git config --global user.email "seu-email@exemplo.com": Define o e-mail do usuário globalmente 
  git config --global user.name "Seu Nome": Define o nome do usuário globalmente 
  git remote add origin [URL]: Conecta o repositório local a um repositório remoto no GitHub 
2. Controle de Versão (Ciclo de Trabalho)
  git status: Verifica o estado dos arquivos no diretório de trabalho (quais estão sendo rastreados ou modificados) 
  git add [arquivo] ou git add .: Adiciona arquivos específicos ou todos os arquivos modificados para a "staging area" 
  git commit -m "mensagem": Cria uma nova versão (commit) com uma mensagem descritiva do que foi feito 
  git push -u origin [branch]: Envia os commits locais para o repositório remoto 
  git pull: Traz as atualizações do servidor remoto para sua máquina local 
3. Navegação e Histórico
  git reflog: Exibe o histórico de todas as alterações e commits realizados 
  git reset --hard [ID_do_commit]: Reverte o código local para um commit específico do histórico 
4. Branches (Ramificações)
  git branch: Lista as branches existentes 
  git branch [nome_da_branch]: Cria uma nova branch 
  git checkout [nome_da_branch]: Alterna para uma branch específica 
  git checkout -b [nome_da_branch]: Cria e alterna para uma nova branch simultaneamente 
  git merge [nome_da_branch]: Une as alterações de uma branch específica na branch atual 
5. Recursos Adicionais
  touch .gitignore: Cria o arquivo de configuração para ignorar arquivos que não devem ser versionados 
  git --help: Exibe a lista de comandos disponíveis do Git 

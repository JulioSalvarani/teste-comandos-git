# 🛠️ Guia Rápido de Comandos Git

Este é um guia de referência rápida para os comandos essenciais do Git, organizados pelo fluxo de trabalho.

---

## 1. Configuração e Inicialização
Comandos iniciais para preparar o seu ambiente de desenvolvimento e conectar com servidores remotos.

* `git init`  
    *Inicializa um novo repositório Git na sua pasta local atual.*
* `git config --global user.name "Seu Nome"`  
    *Define o seu nome de usuário globalmente para identificar seus commits.*
* `git config --global user.email "seu-email@exemplo.com"`  
    *Define o seu e-mail globalmente.*
* `git remote add origin [URL]`  
    *Conecta o seu repositório local a um repositório remoto (ex: GitHub).*

---

## 2. Controle de Versão (Ciclo de Trabalho)
O fluxo diário de desenvolvimento: monitorar, preparar, salvar e sincronizar alterações.

| Comando | Descrição |
| :--- | :--- |
| `git status` | Verifica o estado atual dos arquivos (quais estão modificados, não rastreados ou na *staging area*). |
| `git add [arquivo]` | Adiciona um arquivo específico para a *staging area* (preparação). |
| `git add .` | Adiciona **todas** as alterações do diretório atual para a *staging area*. |
| `git commit -m "mensagem"` | Salva as alterações preparadas criando uma nova versão (commit) com uma mensagem descritiva. |
| `git push -u origin [branch]` | Envia os commits locais para o repositório remoto e define a branch padrão para futuros pushes. |
| `git pull` | Traz e mescla de forma automática as atualizações do servidor remoto para a sua máquina local. |

---

## 3. Branches (Ramificações)
Gerencie diferentes linhas de desenvolvimento e recursos de forma isolada.

* **Listar branches:**
    ```bash
    git branch
    ```
* **Criar uma nova branch:**
    ```bash
    git branch [nome_da_branch]
    ```
* **Alternar para uma branch existente:**
    ```bash
    git checkout [nome_da_branch]
    ```
* **Criar e alternar imediatamente:**
    ```bash
    git checkout -b [nome_da_branch]
    ```
* **Mesclar alterações:**
    ```bash
    git merge [nome_da_branch]
    ```
    *Une as alterações da branch especificada na branch onde você está atualmente.*

---

## 4. Navegação e Histórico
Comandos para consultar o passado do projeto e realizar manobras de recuperação.

* `git reflog`  
    *Exibe o histórico completo de todas as ações, movimentações de HEAD e alterações locais (mesmo as que não estão no histórico normal).*
* `git reset --hard [ID_do_commit]`  
    *⚠️ **Cuidado:** Reverte completamente o código local e descarta todas as alterações após o commit específico informado.*

---

## 5. Recursos Adicionais

* `touch .gitignore`  
    *Cria o arquivo de configuração usado para listar arquivos e pastas que o Git deve ignorar (como chaves de API, senhas ou pastas `node_modules`).*
* `git --help`  
    *Abre a documentação oficial com a lista completa de comandos disponíveis no Git.*

---

💡 *Dica: Sempre execute `git status` antes de fazer um commit para garantir que está salvando exatamente o que deseja!*

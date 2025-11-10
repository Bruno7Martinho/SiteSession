Sistema de Login com Cookies e Sessions
Um exemplo prático de sistema de autenticação usando PHP com sessões e cookies para a funcionalidade "Lembrar-me".

📁 Estrutura do Projeto

login-exemplo/

│

├── login.php          ← Página de login com formulário

├── validar.php        ← Processa e valida as credenciais

├── dashboard.php      ← Página protegida (requer login)

└── sair.php           ← Finaliza a sessão do usuário
🚀 Funcionalidades
Sistema de Login: Autenticação de usuário

Sessões PHP: Mantém o usuário logado durante a navegação

Cookies: Funcionalidade "Lembrar-me" para salvar o nome de usuário

Página Protegida: Dashboard acessível apenas para usuários autenticados

Logout: Finalização segura da sessão

🔧 Tecnologias Utilizadas
PHP 7.4+ - Backend e gerenciamento de sessões

HTML5 - Estrutura das páginas

CSS3 - Estilização e design responsivo

Sessions PHP - Autenticação de usuário

Cookies - Lembrar credenciais do usuário

📋 Requisitos
Servidor web (Apache, Nginx, etc.)

PHP 7.4 ou superior

Habilitada a extensão de sessões no PHP

🔐 Credenciais de Teste
Usuário: admin

Senha: 1234

🛠️ Como Usar
Clone ou baixe os arquivos para o diretório do seu servidor web

Acesse o projeto através do navegador: http://localhost/login-exemplo/

Faça login usando as credenciais de teste

Experimente a funcionalidade "Lembrar-me" para ver os cookies em ação

Teste o logout para finalizar a sessão

📖 Explicação do Código
login.php
Formulário de login com campos para usuário e senha

Checkbox "Lembrar-me" para persistência de login

Exibe mensagens de erro de autenticação

Preenche automaticamente o usuário se existir cookie

validar.php
Valida as credenciais do usuário

Cria sessão em caso de sucesso

Gerencia cookies baseado na opção "Lembrar-me"

Redireciona para dashboard ou retorna erro

dashboard.php
Página protegida que verifica a sessão

Exibe informações do usuário logado

Mostra se a opção "Lembrar-me" está ativa

Botão para logout

sair.php
Destrói a sessão do usuário

Redireciona para a página de login

🔒 Segurança
Uso de htmlspecialchars() para prevenir XSS

Verificação de sessão em páginas protegidas

Destruição adequada de sessões no logout

Cookies configurados com path específico

⚙️ Personalização
Para usar em produção:

Altere as credenciais no arquivo validar.php

Implemente validação mais robusta de senhas

Adicione conexão com banco de dados

Implemente proteção contra ataques de força bruta

Use HTTPS para maior segurança

📝 Notas
Os cookies são configurados para durar 30 dias

A sessão é destruída completamente no logout

As mensagens de erro são limpas após serem exibidas

O projeto usa estilização CSS inline para facilidade de uso

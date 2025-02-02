# Projeto Laravel

Este repositório contém a base de um projeto desenvolvido com o framework Laravel. O projeto foi criado para ser mais rápido e fácil criar um novo projeto laravel.


## Pré-requisitos

Antes de começar, certifique-se de ter os seguintes softwares instalados em sua máquina:

- [PHP](https://www.php.net/downloads.php) (versão 8.0 ou superior)
- [Composer](https://getcomposer.org/) (para gerenciamento de dependências)
- [Git](https://git-scm.com/) (para controle de versão)
- [Banco de Dados] (MySQL, PostgreSQL, SQLite, etc.) - [Instale conforme necessário]

## Instalação

Siga os passos abaixo para configurar o projeto localmente:

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/Felipe-dev01/nome-do-repositorio.git
   cd nome-do-repositorio
   ```

2. **Instale as dependências do PHP**:
   ```bash
   composer install
   ```

3. **Configure o ambiente**:
   - Copie o arquivo `.env.example` para `.env`:
     ```bash
     cp .env.example .env
     ```
   - Abra o arquivo `.env` e configure as variáveis de ambiente, como `DB_DATABASE`, `DB_USERNAME`, `DB_PASSWORD`, etc.

4. **Gere a chave da aplicação**:
   ```bash
   php artisan key:generate
   ```

5. **Execute as migrações do banco de dados**:
   ```bash
   php artisan migrate
   ```

6. **(Opcional) Popule o banco de dados com dados de teste**:
   ```bash
   php artisan db:seed
   ```

7. **Compile os assets front-end**:
   ```bash
   npm run dev
   ```

8. **Inicie o servidor de desenvolvimento**:
   ```bash
   php artisan serve
   ```

9. **Acesse a aplicação**:
    Abra o navegador e acesse:
    ```
    http://localhost:8000
    ```

---

## Estrutura do Projeto

A estrutura do projeto segue o padrão do Laravel:

```
nome-do-repositorio/
├── app/                  # Contém a lógica da aplicação (models, controllers, etc)
├── bootstrap/            # Arquivos de inicialização do framework
├── config/               # Arquivos de configuração
├── database/             # Migrações, seeders e factories
├── public/               # Pasta pública (assets compilados, index.php)
├── resources/            # Views, assets não compilados (CSS, JS)
├── routes/               # Rotas da aplicação
├── storage/              # Armazenamento de arquivos (logs, cache, etc.)
├── .editorconfig         # Configurações de estilo de código
├── .env.example          # Exemplo de variáveis de ambiente
├── .gitattributes        # Configurações do Git
├── .gitignore            # Arquivos e pastas ignorados pelo Git
├── artisan               # CLI do Laravel
├── composer.json         # Configuração do Composer
├── package.json          # Configuração do Node.js
├── phpunit.xml           # Configuração do PHPUnit para testes
├── postcss.config.js     # Configuração do PostCSS para estilos
└── README.md             # Documentação do projeto
```

---

## Comandos Úteis

Aqui estão alguns comandos úteis para trabalhar com o projeto:

- **Limpar cache**:
  ```bash
  php artisan cache:clear
  php artisan config:clear
  php artisan route:clear
  php artisan view:clear
  ```

- **Criar um novo controller**:
  ```bash
  php artisan make:controller NomeDoController
  ```

- **Criar uma nova migration**:
  ```bash
  php artisan make:migration nome_da_migration
  ```

---

## Contribuição

Contribuições são bem-vindas! Siga os passos abaixo para contribuir:

10. Faça um fork do projeto.
11. Crie uma branch para sua feature ou correção:
   ```bash
   git checkout -b feature/nova-funcionalidade
   ```
12. Commit suas mudanças:
   ```bash
   git commit -m 'Adicionando nova funcionalidade'
   ```
13. Push para a branch:
   ```bash
   git push origin feature/nova-funcionalidade
   ```
14. Abra um Pull Request no GitHub.

---

## Contato

Se você tiver dúvidas ou sugestões, sinta-se à vontade para entrar em contato:

- **Nome**: Felipe T. Farias
- **GitHub**: [Felipe-dev01](https://github.com/Felipe-dev01)

---

### Notas Adicionais

- Certifique-se de configurar corretamente o arquivo `.env` com as credenciais do banco de dados.
- Se você encontrar algum problema, verifique os logs em `storage/logs/` para mais detalhes.

---

# Laravel-Backend

API em Laravel para o CRUD de produtos.

Tarefas:
- Criar API
- Criar CRUD de produtos (nome, descrição, marca, preço, estoque)
- Usar MySQL

1. Pré-requisitos
PHP 8.2+
Composer
MySQL
XAMPP (opcional)
2. Clonar o repositório
git clone https://github.com/FelipeCagnin2007/Laravel-Backend.git

Abra o projeto em um editor de arquivos, como o VSCode:

cd Laravel-Backend

3. Instalar dependências
composer install

4. Configurar ambiente
Renomeie o arquivo .env.example para .env e ajuste as configurações do banco:
Altere no .env, removendo os asteriscos:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel   //Nome utilizado no exemplo!
DB_USERNAME=root
DB_PASSWORD=

5. Criar a chave da aplicação
php artisan key:generate

6. Criar banco de dados e tabelas
php artisan migrate
Would you like to create it? (yes/no) Escolha a opção Yes (Y)

7. Rodar a API
php artisan serve

A API ficará disponível em:
http://127.0.0.1:8000

8. Testar endpoints
Se desejar, use Insomnia, Postman ou outro cliente HTTP para testar:
GET /api/produtos – listar produtos
POST /api/produtos – criar produto
GET /api/produtos/{id} – ver produto específico
PUT /api/produtos/{id} – atualizar produto
DELETE /api/produtos/{id} – deletar produto

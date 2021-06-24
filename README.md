# MySQL Server Alura

👋 Olá, Seja Bem-vindo(a) ao 'Design Patterns Python II: Boas práticas de programação'.

# Projeto 'MySQL Server Alura' do curso:

## [Introdução ao SQL com MySQL: Manipule e consulte dados](https://cursos.alura.com.br/course/mysql-manipule-dados-com-sql)

# Aulas

<details>
    <summary>Instalando e configurando o MYSQL</summary>
    <ul>
        <li>Introdução</li>
        <li>História do SQL</li>
        <li>História do MySQL</li>
        <li>Instalando o MySQL Server</li>
        <li>Consolidando o seu conhecimento</li>
        <li>O que aprendemos?</li>
    </ul>
</details>

<details>
    <summary>Manipulando o banco de dados</summary>
    <ul>
        <li>Definições</li>
        <li>Localização da tabela</li>
        <li>Componentes de tabelas</li>
        <li>Agrupando tabelas</li>
        <li>Conhecendo o Workbench</li>
        <li>Criando um banco de dados</li>
        <li>Comando para criação de banco de dados</li>
        <li>Criando um banco de dados usando assistente</li>
        <li>Criando um banco de dados</li>
        <li>Apagando banco de dados</li>
        <li>Exclusão de um banco de dados</li>
        <li>MYSQL por linha de comando</li>
        <li>Consolidando o seu conhecimento</li>
        <li>O que aprendemos?</li>
    </ul>
</details>

<details>
    <summary>Gerenciando as tabelas do banco de dados</summary>
    <ul>
        <li>Tipos de dados</li>
        <li>Tipo data</li>
        <li>Criando a primeira tabela</li>
        <li>Criando tabela de vendedores</li>
        <li>Criando a tabela pelo assistente</li>
        <li>Apagando tabelas</li>
        <li>Apagando a tabela de vendedores</li>
        <li>Consolidando o seu conhecimento</li>
        <li>O que aprendemos?</li>
    </ul>
</details>

<details>
    <summary>Manutenção dos dados nas tabelas</summary>
    <ul>
        <li>Inserindo registros na tabela</li>
        <li>Incluindo o primeiro vendedor</li>
        <li>Inserindo vários registros na tabela</li>
        <li>Incluindo mais dois vendedores</li>
        <li>Alterando registros</li>
        <li>Alterando informações sobre os vendedores</li>
        <li>Excluindo registros</li>
        <li>Excluindo vendedor</li>
        <li>Incluindo a chave primária</li>
        <li>Comando para criação da chave primária</li>
        <li>Manipulando datas e campos lógicos</li>
        <li>Modificando a tabela de Vendedores</li>
        <li>Consolidando o seu conhecimento</li>
        <li>O que aprendemos?</li>
    </ul>
</details>

<details>
    <summary>Consultando os dados</summary>
    <ul>
        <li>Incluindo dados na tabela</li>
        <li>Selecionando todos os vendedores</li>
        <li>Filtrando registros</li>
        <li>Selecionando um vendedor</li>
        <li>Filtrando usando maior, menor e diferente</li>
        <li>Selecionando vendedor pelo valor da comissão</li>
        <li>Filtrando datas</li>
        <li>Selecionando vendedor pela data</li>
        <li>Filtros compostos</li>
        <li>Seleção composta</li>
        <li>Consolidando o seu conhecimento</li>
        <li>O que aprendemos?</li>
        <li>Conclusão</li>
    </ul>
</details>

# Notas das aulas:

# Sobre o projeto:

### Permissões de arquivos:

Ao se criar migrações, adicionar libs ou qualquer outro comando que crie arquivos dentro do contâiner Docker o proprietário para edição se torna o contâiner, sendo assim você precisará rodar o comando abaixo para alterar essas permissões e você poder editar:

```sh
sudo chown -R $USER:$USER .
```

# Exigências

**:warning: Atenção:** É necessário que os desenvolvedores usem o Docker no seu ambiente de desenvolvimento.

- **🛠 Modo Desenvolvimento Docker**
    - :computer: [Linux Ubuntu LTS](https://ubuntu.com/download/desktop)
    - 🐳 [Docker](https://docs.docker.com/engine/installation/) Deve estar instalado.
    - 🐳 [Docker Compose](https://docs.docker.com/compose/) Deve estar instalado.
    - **💡 Dica:** [Documentação do Docker](https://docs.docker.com/)

# Instalando

## 🐳 Modo Desenvolvimento com Docker

Após instalar o docker e docker-compose, estando na pasta raiz do projeto, execute:

```sh
docker-compose up
```

Para se certificar que os seus containers subiram corretamente, todos os containers deve estar com o status `UP`, execute:

```sh
docker-compose ps -a
```

Para acessar o container da aplicação, execute:

```sh
docker-compose run --rm app bash
```

Para derrubar e subir a instância do docker novamente, execute:

```sh
docker-compose down && docker-compose up
```

## Acessar o banco:
```sh
1° [dentro do container] - Subir o banco:
docker-compose up -d db

2° [dentro do container] - Listar container:
docker ps

3° [dentro do container] - Entrar no container:
docker exec -it [id do db] bash

5° [dentro do container] - Entrar no banco:
mysql -u root -psecret alura

6° [dentro do container] - Sair de dentro do banco de desenvolvimento:
 CRTL + D
```

# Referências utilizadas

[1° Handy MySQL Commands](http://g2pc1.bu.edu/~qzpeng/manual/MySQL%20Commands.htm)

# Pomodoro Backend

Este é o backend da aplicação Pomodoro, construído com Strapi.

## Requisitos

- Node: >=10.16.0 <=14.x.x
- NPM: ^6.0.0
- Docker

## Configuração inicial

### Docker e PostgreSQL

Para rodar este projeto localmente, você precisa ter o Docker instalado. Vamos usar o Docker para criar um container com a imagem do PostgreSQL. 

1. **Puxe a imagem do PostgreSQL**:
```bash 
docker pull postgres 
```

2. **Inicie o container do PostgreSQL:**
```bash 
docker run --name pomodoro-postgres -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=root -e POSTGRES_DB=postgres -p 5432:5432 -d postgres
```

Este comando inicia um novo container chamado "pomodoro-postgres" usando a imagem do PostgreSQL, e configura as variáveis de ambiente para o usuário, senha e banco de dados. Ele também mapeia a porta 5432 do container para a porta 5432 do seu host.

### Instalação e Execução do Projeto
3. **Clone o repositório**:
```bash 
git clone https://github.com/MatheusDourado/api_pomodoro.git 
```

4. **Navegue até a pasta do projeto**:
```bash 
cd api_pomodoro
```

5. **Execute o projeto**:
```bash 
npm run develop
```
Isso iniciará o servidor Strapi e você poderá acessá-lo em http://localhost:1337.

##### **Licença** Mit

Desenvolvido com 💙 por Matheus Dourado

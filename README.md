# alimentos_taco
Api de alimentos da tabela TACO utilizando o framework vaden
## Documentação da API
A documentação da API [localhost:8080/docs](http://localhost:8080/docs/).
## Rodando a aplicação  
1. Subindo os postgres via docker
   ```bash
   docker run -d --name alimentoTacoDb -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=senha123 -e POSTGRES_DB=alimento_taco -v postgres_data:/var/lib/postgresql/data -p 5432:5432 postgres:latest
   ```
2. Clonar repositório
   ```bash
   git clone https://github.com/fabiovinicius1/alimentos_taco.git
   ```
3. Navegando para o repositório
   ```bash
   cd alimentos_taco/
   ```
4. Instale as Dependências (Necessário que o Dart esteja na versão 3.7.2)
   ```bash
   dart pub get
   ```
5. Execute o Scanner de Classes com build_runner
   ```bash
   dart run build_runner watch
   ```
6. Executando o Projeto
   ```bash
   dart run bin/server.dart
   ```


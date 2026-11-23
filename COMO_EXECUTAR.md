# Executar a cópia da demonstração

1. Instale o JDK 17 e o MySQL e importe o dump recebido separadamente.
2. Mantenha backend e frontEnd lado a lado. Preserve backend/data/arquivos: essa pasta contém as capas e o PDF demonstrativo referenciados pelo banco.
3. No CMD, entre na pasta backend e execute:

```bat
copy src\main\resources\application-example.properties src\main\resources\application.properties
mvnw.cmd spring-boot:run
```

Faça a cópia da configuração apenas na primeira execução, se application.properties ainda não existir.
4. Abra http://localhost:8080 e configure a conexão com o MySQL que contém o dump. Use as credenciais do computador de destino.
5. Entre com uma conta que já seja administradora no dump. Em Minha biblioteca, ajuste nome e endereço do site. Para acesso público, execute o ngrok no computador que hospeda o backend; preencher o endereço não inicia o túnel.

O backend também serve o frontend. Execute sempre a partir da pasta backend para que os caminhos relativos dos arquivos sejam encontrados.

O PDF é apenas um exemplo para apresentação, não o conteúdo integral dos livros. Senhas de conexão, bancos locais, backups e configurações pessoais não acompanham este repositório. Os dados de usuários e empréstimos vêm do dump recebido separadamente.

# Green Dinner - Gestão de Clientes

Este projeto implementa um sistema simples de cadastro, consulta, exclusão e atualização de clientes usando Java e uma interface gráfica com `JOptionPane`. Os dados do cliente incluem nome, CPF, telefone, endereço, número, cidade e estado.

## Funcionalidades

- **Cadastro de Clientes**: Insere novos clientes no sistema.
- **Consulta de Clientes**: Consulta os clientes cadastrados pelo CPF.
- **Exclusão de Clientes**: Exclui clientes do sistema pelo CPF.
- **Atualização de Clientes**: Atualiza os dados de clientes já cadastrados.
- **Listagem de Clientes**: Exibe todos os clientes cadastrados ao encerrar a aplicação.

## Tecnologias Utilizadas

- Java
- Swing (JOptionPane)
- Padrão DAO (Data Access Object)

## Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/usuario/repo.git
```

2. Compile o projeto:

```bash
javac -d bin -sourcepath src src/Wellington/henrique/App.java
```

3. Execute a aplicação:

```bash
java -cp bin Wellington.henrique.App
```

4. No menu interativo, você poderá escolher uma das seguintes opções:

- `1`: Cadastro de Cliente
- `2`: Consulta de Cliente
- `3`: Exclusão de Cliente
- `4`: Atualização de Cliente
- `5`: Sair da aplicação

## Estrutura do Projeto

```bash
src/
├── Wellington/
│   ├── henrique/
│   │   ├── App.java          # Classe principal que executa o sistema
│   │   ├── domain/
│   │   │   └── Cliente.java  # Classe Cliente representando os dados
│   │   ├── DAO/
│   │   │   ├── IClienteDAO.java   # Interface DAO
│   │   │   ├── ClienteSetDAO.java # Implementação do DAO usando Set
│   │   │   └── ClienteMapDAO.java # Implementação do DAO usando Map (não utilizado atualmente)
```

## Exemplo de Cadastro

Quando você escolhe a opção de cadastro, será solicitado que informe os dados do cliente no seguinte formato:

```
Nome, CPF, Telefone, Endereço, Número, Cidade, Estado
```

Exemplo:

```
João Silva,12345678901,11987654321,Rua Exemplo,100,São Paulo,SP
```

## Licença

Este projeto está licenciado sob a licença [MIT](LICENSE).

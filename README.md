# Cadastro de Clientes com Tipos Genéricos

Este projeto demonstra a implementação de um cadastro de clientes utilizando conceitos de **tipos genéricos** em Java. Foi desenvolvido com foco na reutilização de código e na segurança de tipos durante a compilação, aproveitando as capacidades avançadas da linguagem Java.

## Estrutura do Projeto

- **IDE Utilizada:** IntelliJ IDEA
- **Versão do Java:** 23
- **Pacote:** `cadastro`
- **Classes:**
  - `ModeloCliente<T, U>`: Classe genérica que armazena os dados do cliente com parâmetros de tipo.
  - `ControleCadastro`: Classe responsável por instanciar e controlar o cadastro dos clientes.

## Funcionalidades

- Cadastro de clientes com os seguintes atributos:
  - Nome (String)
  - Sobrenome (String)
  - Idade (Integer)
  - Endereço (String)
  - E-mail (String)
- Utilização de **parâmetros genéricos** para maior flexibilidade.
- Impressão dos dados cadastrados no console.

## Exemplo de Código

### Classe ModeloCliente
```java
public class ModeloCliente<T, U> {
    private T nome;
    private T sobrenome;
    private U idade;
    private T endereco;
    private T email;

    public ModeloCliente(T nome, T sobrenome, U idade, T endereco, T email) {
        this.nome = nome;
        this.sobrenome = sobrenome;
        this.idade = idade;
        this.endereco = endereco;
        this.email = email;
    }

    @Override
    public String toString() {
        return "Cliente [Nome=" + nome + ", Sobrenome=" + sobrenome +
               ", Idade=" + idade + ", Endereço=" + endereco +
               ", E-mail=" + email + "]";
    }
}
Classe ControleCadastro
java
public class ControleCadastro {
    public static void main(String[] args) {
        ModeloCliente<String, Integer> cliente = new ModeloCliente<>(
            "João", "Silva", 30, "Rua das Flores, 123", "joao.silva@email.com"
        );

        System.out.println(cliente.toString());
    }
}
Requisitos
Java SE 23

IntelliJ IDEA (ou outra IDE com suporte para projetos Java)

Sistema operacional compatível (Windows, macOS ou Linux)

Como Executar
Clone este repositório:

bash
git clone https://github.com/davidMarostica/usar-conceito-gen-rico-UFBRA-.git
Abra o projeto na IDE IntelliJ IDEA.

Certifique-se de que a versão do JDK 23 está configurada no projeto.

Execute a classe ControleCadastro para inicializar o programa.

Resultado Esperado
A saída no console será algo como:

Cliente [Nome=João, Sobrenome=Silva, Idade=30, Endereço=Rua das Flores, 123, E-mail=joao.silva@email.com]
Contribuição
Contribuições são bem-vindas! Siga as boas práticas de desenvolvimento e abra uma issue ou envie um pull request com as suas melhorias.

Este README reflete o uso de termos técnicos apropriados e informações relevantes sobre o ambiente de desenvolvimento. Se precisar de ajustes ou acréscimos, é só avisar! 🚀

e para cria um README para colocar o gitub esplicando o projeto em questao
Baseado no projeto de cadastro de clientes com tipos genéricos e levando em consideração a estrutura típica de um README para o GitHub, aqui está um modelo que você pode usar para explicar seu projeto:

markdown
# Cadastro de Clientes com Tipos Genéricos

Este repositório contém uma aplicação simples de cadastro de clientes, desenvolvida em **Java** utilizando o conceito de **tipos genéricos**. O objetivo deste projeto é demonstrar como aplicar a programação genérica para criar código reutilizável, eficiente e seguro em tempo de compilação.

## 🚀 Tecnologias Utilizadas

- **Linguagem:** Java 23
- **IDE:** IntelliJ IDEA
- **Versionamento:** Git e GitHub

## 📂 Estrutura do Projeto

- **Pacote:** `cadastro`
- **Classes:**
  - `ModeloCliente<T, U>`: Uma classe genérica que armazena dados dos clientes.
  - `ControleCadastro`: Classe que controla a execução do programa, instanciando a `ModeloCliente` e exibindo as informações no console.

## 📋 Funcionalidades

- Cadastro de clientes com os seguintes atributos:
  - Nome
  - Sobrenome
  - Idade
  - Endereço
  - E-mail
- Utilização de **parâmetros genéricos** para maior flexibilidade e segurança de tipos.
- Impressão dos dados do cliente no console.

## 🧩 Exemplo de Código

### Classe ModeloCliente
```java
public class ModeloCliente<T, U> {
    private T nome;
    private T sobrenome;
    private U idade;
    private T endereco;
    private T email;

    public ModeloCliente(T nome, T sobrenome, U idade, T endereco, T email) {
        this.nome = nome;
        this.sobrenome = sobrenome;
        this.idade = idade;
        this.endereco = endereco;
        this.email = email;
    }

    @Override
    public String toString() {
        return "Cliente [Nome=" + nome + ", Sobrenome=" + sobrenome +
               ", Idade=" + idade + ", Endereço=" + endereco +
               ", E-mail=" + email + "]";
    }
}
Classe ControleCadastro
java
public class ControleCadastro {
    public static void main(String[] args) {
        ModeloCliente<String, Integer> cliente = new ModeloCliente<>(
            "João", "Silva", 30, "Rua das Flores, 123", "joao.silva@email.com"
        );

        System.out.println(cliente.toString());
    }
}
🛠️ Como Executar
Clone este repositório:

bash
git clone https://github.com/davidMarostica/usar-conceito-gen-rico-UFBRA-.git
Abra o projeto na IDE IntelliJ IDEA.

Configure a versão do JDK como Java 23.

Execute a classe ControleCadastro para rodar o programa.

📋 Resultado Esperado
Ao executar o programa, o console exibirá:

Cliente [Nome=David, Sobrenome=Silva, Idade=41, Endereço=Rua das Flores, 123, E-mail=david.silva@email.com]
🤝 Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request com suas melhorias ou sugestões.

Autor: Desenvolvido por David Marostica. Licença: Este projeto está licenciado sob os termos da licença MIT.# usar-conceito-gen-rico-UFBRA-

# 🌦️ Sistema de Informações Climáticas em Tempo Real

Aplicação desenvolvida em Java para consultar informações meteorológicas
atuais de uma cidade utilizando a API WeatherAPI.

## 📌 Sobre o Projeto

O Sistema de Informações Climáticas em Tempo Real é um projeto desenvolvido
em Java com o objetivo de praticar conceitos de programação e integração
com APIs externas.

A aplicação solicita ao usuário o nome de uma cidade, realiza uma requisição
HTTP à WeatherAPI e processa os dados meteorológicos recebidos no formato JSON.

Este projeto faz parte da minha jornada de aprendizado em Java e do
desenvolvimento de aplicações práticas.

## 🚀 Funcionalidades

- 🔎 Consulta de informações meteorológicas pelo nome da cidade.
- 🌎 Exibição do nome da cidade e do país.
- 🌡️ Consulta da temperatura atual em graus Celsius.
- 🌡️ Exibição da sensação térmica.
- 🌤️ Identificação da condição climática.
- 💧 Consulta da umidade relativa do ar.
- 💨 Exibição da velocidade do vento em km/h.
- 🌬️ Consulta da pressão atmosférica em milibares.
- 🕒 Exibição da data e hora da última atualização meteorológica.
- ⚠️ Tratamento básico de erros retornados pela API.

## 🛠️ Tecnologias Utilizadas

- **Java 11 ou superior:** linguagem de programação utilizada no projeto.
- **HttpClient:** realização de requisições HTTP.
- **WeatherAPI:** fornecimento dos dados meteorológicos.
- **org.json:** interpretação e manipulação de dados JSON.
- **Git e GitHub:** versionamento e hospedagem do código-fonte.

## 📋 Pré-requisitos

Para executar o projeto, você precisará de:

- Java Development Kit (JDK) 11 ou superior.
- Biblioteca `org.json`.
- Uma conta na WeatherAPI.
- Uma chave de API válida.

## ⚙️ Configuração do Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/NathaRosa/-real-time-climate-information-system.git
```

Entre no diretório do projeto:

```bash
cd -real-time-climate-information-system
```

### 2. Configure a chave da API

Acesse o site da [WeatherAPI](https://www.weatherapi.com/) e obtenha
uma chave de API.

Na pasta em que o programa será executado, crie um arquivo chamado:

`api-key.txt`

Adicione sua chave ao arquivo:

```text
SUA_CHAVE_API
```

Substitua `SUA_CHAVE_API` pela chave obtida na WeatherAPI.

**Importante:** não compartilhe sua chave nem a publique no GitHub.

Certifique-se de que o arquivo `api-key.txt` esteja incluído no
`.gitignore`.

### 3. Configure a biblioteca JSON

Certifique-se de que a biblioteca `org.json` esteja disponível no
classpath do projeto.

Caso utilize um arquivo JAR chamado `json.jar`, coloque-o no diretório
principal do projeto ou ajuste os comandos abaixo para indicar o caminho
correto.

### 4. Compile o programa

Considerando que o arquivo Java esteja dentro da pasta `src` e que a
biblioteca esteja disponível como `json.jar` no diretório principal:

```bash
javac -cp ".:json.jar" -d out src/ProjetoSistemaDeInformacoesClimaticasEmTempoReal.java
```

Se a estrutura do projeto for diferente, ajuste os caminhos conforme
necessário.

### 5. Execute a aplicação

Execute o programa a partir do diretório principal do projeto:

```bash
java -cp "out:json.jar" ProjetoSistemaDeInformacoesClimaticasEmTempoReal
```

Os comandos podem variar conforme a configuração do ambiente de
desenvolvimento e a localização da biblioteca JSON.

## 💻 Exemplo de Utilização

Ao iniciar a aplicação, o programa solicita o nome da cidade desejada.

```text
Digite o nome da cidade: Itu
```

Quando a API retorna uma resposta válida, a aplicação apresenta
informações meteorológicas, incluindo:

- Cidade e país.
- Data e hora da última atualização.
- Temperatura atual.
- Sensação térmica.
- Condição climática.
- Umidade do ar.
- Velocidade do vento.
- Pressão atmosférica.

Os valores apresentados dependem das informações retornadas pela API
no momento da consulta.

## 📚 Conceitos Praticados

Durante o desenvolvimento deste projeto, são praticados conceitos
importantes da programação Java:

- Organização do código em métodos.
- Entrada de dados com `Scanner`.
- Leitura de arquivos com `Files` e `Paths`.
- Codificação de parâmetros de URL com `URLEncoder`.
- Requisições HTTP com `HttpClient`.
- Tratamento de respostas HTTP com `HttpResponse`.
- Interpretação de JSON com `JSONObject`.
- Tratamento de exceções com `try-catch`.
- Integração com APIs REST.
- Gerenciamento básico de chaves de API.

## 🔮 Melhorias Futuras

Algumas melhorias que poderão ser implementadas:

- Aprimorar o tratamento de erros da API.
- Validar os nomes das cidades informadas.
- Permitir consultas consecutivas sem reiniciar o programa.
- Melhorar o gerenciamento das credenciais.
- Implementar testes automatizados.
- Desenvolver uma interface gráfica.
- Adicionar novas informações meteorológicas.

## 👨‍💻 Autor

**NathaRosa**

GitHub: [@NathaRosa](https://github.com/NathaRosa)

---

Projeto desenvolvido para fins educacionais, como parte do meu
aprendizado em Java e desenvolvimento de software.

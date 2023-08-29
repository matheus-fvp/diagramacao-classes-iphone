# Modelagem e diagramação da representação em UML e código no que se refere ao componente Iphone 

# Sobre o projeto
Este projeto tem por objetivo desenvolver um protótipo simples do Iphone utilizando os conceitos de POO, para tanto foi necessária a modelagem e diagramação da representação do IPhone em UML

# Diagrama de classes UML

```mermaid
classDiagram
class ReprodutorMusical {
  <<interface>>
  +tocar() void
  +pausar() void
  +selecionarMusica(String musica) void
}
class AparelhoTelefonico {
  <<interface>>
  +ligar(String numero) void
  +atender() void
  +iniciarCorreioVoz(int posicao) void
}

class Navegador {
  <<interface>>
  +exibirPagina(String pagina) void
  +adicionarNovaAba(String aba) void
  +atualizarPagina() void
}

class Iphone {
  -Set~String~ musicas
  +getMusicas() Set~String~
}

ReprodutorMusical <|.. Iphone
AparelhoTelefonico <|.. Iphone
Navegador <|.. Iphone 
```

# Tecnologias utilizadas 
  - Java JDK 17
  - IntelliJ IDEA

# Como executar o projeto
Pré-requisitos: Java JDK 17

# Autor
Matheus Fernando Vieira Pinto.

https://www.linkedin.com/in/matheus-vieira-06166722a/

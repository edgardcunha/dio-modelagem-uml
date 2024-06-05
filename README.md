# dio-modelagem-uml
Repositório com o código do desafio "Modelando o iPhone com UML: Funções de Músicas, Chamadas e Internet".

### Diagrama UML
```mermaid
classDiagram
    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class NavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class SmartPhone {
      <<Abstract>>
    }

    class iPhone {
    }

    SmartPhone <|-- iPhone
    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet
```

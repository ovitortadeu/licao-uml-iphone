# licao-uml-iphone

```mermaid
---
config:
  theme: dark
  look: classic
  layout: dagre
---
classDiagram
direction TB
    class Iphone {
    }
    class ReprodutorMusical {
	    +tocar() String
	    +pausar() String
	    +selecionarMusica(String musica) String
    }
    class AparelhoEletronico {
	    +ligar(String numero) String
	    +atender() String
	    +iniciarCorreioVoz() String
    }
    class NavegadorInternet {
	    +exibirPagina(String url) String
	    +adicionarNovaAba() String
	    +atualizarPagina() String
    }
    class Telefone {
	    -telefone: int
	    -contatos: ArrayList
	    +ligar(String numero) String
	    +atender() String
	    +iniciarCorreioVoz() String
    }
    class Buscador {
	    -historico: ArrayList
	    +exibirPagina(String url) String
	    +adicionarNovaAba() String
	    +atualizarPagina() String
    }
    class Ipod {
	    -albuns: String
	    -artistas: String
	    -musicas: String
        +tocar() String
	    +pausar() String
	    +selecionarMusica(String musica) String
    }

	<<Interface>> ReprodutorMusical
	<<Interface>> AparelhoEletronico
	<<Interface>> NavegadorInternet

    Iphone --|> ReprodutorMusical
    Iphone --|> AparelhoEletronico
    Iphone --|> NavegadorInternet
    AparelhoEletronico <|-- Telefone
    NavegadorInternet <|-- Buscador
    ReprodutorMusical <|-- Ipod
```



### Minha lógica
Fiz o que foi pedido
1. **Reprodutor Musical**
   - Métodos: `tocar()`, `pausar()`, `selecionarMusica(String musica)`
2. **Aparelho Telefônico**
   - Métodos: `ligar(String numero)`, `atender()`, `iniciarCorreioVoz()`
3. **Navegador na Internet**
   - Métodos: `exibirPagina(String url)`, `adicionarNovaAba()`, `atualizarPagina()`
e criei as respectivas classes para as interfaces acima, com seus atributos que julguei serem importantes.

# Exemplo de Generics em Java

Este projeto contém um exemplo simples de como usar Generics em Java para garantir a segurança de tipos em coleções. 

## Descrição

O exemplo demonstra a diferença entre o uso de coleções com e sem Generics, e como isso afeta a segurança e a necessidade de fazer casting ao iterar sobre os elementos da lista.

## Estrutura do Código

- **Pacote:** `collections`
- **Classe:** `GenerucsExempleList`

### Funcionalidades

1. **Exemplo sem Generics:**
   - Criação de uma lista (`ArrayList`) sem especificar o tipo de elementos.
   - Adição de elementos de tipos diferentes (String e Integer).
   - Necessidade de casting ao iterar sobre a lista.

2. **Exemplo com Generics:**
   - Criação de uma lista (`ArrayList<String>`) especificando que apenas Strings podem ser adicionadas.
   - Adição de elementos do tipo String.
   - Iteração segura sobre a lista sem necessidade de casting.
  

   # Desafio diagramação das funcionalidades do iPhone 2007


```mermaid
classDiagram
    class iPhone {
        - modelo: String
        - versaoOS: String
        - numeroDeSerie: String
        + ligar()
        + desligar()
        + desbloquear()
        + bloquear()
    }
    class Telefone {
        - listaContatos: List
        - historicoChamadas: List
        + fazerChamada()
        + receberChamada()
        + adicionarContato()
        + removerContato()
        + verHistoricoChamadas()
    }
    class Mensagens {
        - listaMensagens: List
        + enviarMensagem()
        + receberMensagem()
        + deletarMensagem()
    }
    class Email {
        - contasEmail: List
        - listaEmails: List
        + enviarEmail()
        + receberEmail()
        + adicionarConta()
        + removerConta()
    }
    class Safari {
        - listaFavoritos: List
        - historicoNavegacao: List
        + navegar()
        + adicionarFavorito()
        + removerFavorito()
        + verHistorico()
    }
    class iPod {
        - listaMusicas: List
        - listaVideos: List
        - playlists: List
        + reproduzirMusica()
        + reproduzirVideo()
        + criarPlaylist()
        + adicionarMusicaPlaylist()
    }
    class Fotos {
        - listaFotos: List
        - listaAlbuns: List
        + tirarFoto()
        + visualizarFoto()
        + criarAlbum()
        + adicionarFotoAlbum()
    }
    class Calendário {
        - eventos: List
        + adicionarEvento()
        + removerEvento()
        + verEvento()
    }
    class Mapas {
        - localizaçãoAtual: String
        - locaisFavoritos: List
        + buscarLocal()
        + obterRota()
        + adicionarFavorito()
        + removerFavorito()
    }
    class Configurações {
        - ajustesRede: Map
        - ajustesSom: Map
        - ajustesBrilho: Map
        + ajustarRede()
        + ajustarSom()
        + ajustarBrilho()
    }

    iPhone --> Telefone
    iPhone --> Mensagens
    iPhone --> Email
    iPhone --> Safari
    iPhone --> iPod
    iPhone --> Fotos
    iPhone --> Calendário
    iPhone --> Mapas
    iPhone --> Configurações



# DEISI Rockstar 

Projeto universitário desenvolvido na **Universidade Lusófona** para a cadeira de **Algoritmos e Estruturas de Dados (AED)**. Consiste num sistema de análise e consulta de dados musicais (estilo Spotify) a partir de ficheiros de texto.

## Estrutura dos Dados

O sistema carrega três ficheiros de dados:

- `songs.txt` — informação base das músicas (ID, título, ano, duração, popularidade, etc.)
- `song_artists.txt` — associação entre músicas e artistas
- `song_details.txt` — detalhes adicionais (dançabilidade, vivacidade, volume médio, letra explícita)

## Comandos Disponíveis

O programa aceita comandos via linha de comandos (terminar com `KTHXBYE`):

| Comando | Descrição |
|---|---|
| `COUNT_SONGS_YEAR <ano>` | Conta músicas lançadas num dado ano |
| `COUNT_DUPLICATE_SONGS_YEAR <ano>` | Conta músicas com título duplicado num dado ano |
| `GET_MOST_DANCEABLE <anoX> <anoY> <N>` | Top N músicas mais dançáveis entre dois anos |
| `GET_TOP_ARTISTS_WITH_SONGS_BETWEEN <N> <A> <B>` | Top N artistas com número de músicas entre A e B |
| `GET_ARTISTS_ONE_SONG <anoIni> <anoFim>` | Artistas com apenas uma música no período |
| `GET_YEAR_HIGHER_DURATION_MUSIC <ano> <min>` | Músicas de um ano com duração ≥ X minutos |
| `ADD_TAGS <artista>;<tag1>;<tag2>...` | Adiciona tags a um artista |
| `REMOVE_TAGS <artista>;<tag1>;<tag2>...` | Remove tags de um artista |
| `GET_ARTISTS_FOR_TAG <tag>` | Lista artistas associados a uma tag |
| `GET_UNIQUE_TAGS` | Lista todas as tags e quantos artistas as usam |
| `GET_UNIQUE_TAGS_IN_BETWEEN_YEARS <anoIni> <anoFim>` | Tags de artistas com músicas no período |
| `CLEANUP` | Remove músicas e artistas sem dados completos |

## Como Executar

1. Clonar o repositório:
   ```bash
   git clone https://github.com/pmrmoreira/projectoAED.git
   ```

2. Colocar os ficheiros `songs.txt`, `song_artists.txt` e `song_details.txt` na raiz do projeto.

3. Compilar e executar a classe `Main` (package `pt.ulusofona.aed.deisiRockstar2021`).

## Tecnologias

- **Java**
- Estruturas de dados: `ArrayList`, `HashMap`, `HashSet`

## Autor

Pedro Moreira — [@pmrmoreira](https://github.com/pmrmoreira)

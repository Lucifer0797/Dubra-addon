# Dubra

Addon para Stremio/Nuvio focado em torrents com áudio PT-BR (dublado/dual).

## Fontes ativas

| Fonte | Método | Cobertura |
|---|---|---|
| Torrentio Brazuca | API | Principal |
| Brazuca Torrents | API | Conteúdo BR |
| BeTor | Prowlarr (recomendado) | Conteúdo BR |
| Torrent Indexer | API | BluDV, Comando, Starck, TorrentDosFilmes, VacaTorrent |
| TorrentsDB | API | Fallback secundário (fonte mista) |

## Regra de idioma

- Fontes BR (Brazuca, BeTor, Indexer e derivados BR): filtro mais leve.
- Fontes mistas (Torrentio/TorrentsDB): filtro PT-BR quando `Idioma original` estiver desligado.

## Interface `/configure`

- Preferências de qualidade/codec/fonte de vídeo com ordenação.
- Fontes ativas.
- Debrid.
- Limites e timeout.
- Status por fonte: `online`, `instável`, `offline`.

## Rodar localmente

```bash
npm install
npm start
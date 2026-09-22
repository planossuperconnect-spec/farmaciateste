# Super Racha (projeto "Racha dos Amigos")

Arquivo principal: `Racha dos Amigos.dc.html` (um único DC com todas as páginas).

## Regras do usuário
- Racha sempre às terças, 20h. Datas conforme calendário real.
- Mudanças pontuais: não alterar layout, design ou outras páginas sem pedido.
- Estilo: fundo escuro (#0f1412), verde (#22c55e / #4ade80), fontes Barlow + Barlow Condensed.
- Logo no cabeçalho: https://i.imgur.com/nw1WEk5.png ("Super Racha").
- Camisas: Time A https://i.imgur.com/fDP8278.jpeg · Time B https://i.imgur.com/YhLya7f.png (object-fit contain, sem fundo).
- Evitar `<img src="{{ hole }}">` (gera erro de console); usar background-image com hole.

## Estado atual (sem banco de dados, tudo em localStorage)
- Navegação: Início, Jogadores, Presença, Times, Partidas, Ranking (key `racha_pagina`).
- Jogadores: CRUD com foto (upload redimensionado), posição, habilidade. Key `racha_jogadores_v2`. Seed: 19 de linha + Gabriel e Diogo goleiros.
- Presença: importar lista do WhatsApp (nomes numerados, "Goleiro: nome", ignora emojis/arbitragem, cria novos sem duplicar). Key `racha_presenca_v1`.
- Times: divisão alternada dos jogadores (demonstrativo).
- Partidas: controle de linha (10 min ou até 2 gols), cronômetro, gols com autor/assistência, tela vermelha "ACABOU O TEMPO", "Iniciar próxima linha", histórico. Keys `racha_partida_v1`, `racha_partidas_hist_v1`.
- Ranking e cartões do Início: dados demonstrativos.

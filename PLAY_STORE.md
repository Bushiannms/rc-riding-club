# RC Riding Club — Google Play: tudo o que precisas

## 1. Ficha da loja

**Nome da app:** RC Riding Club

**Descrição curta (PT, máx. 80):**
Motas, missões e malta: faz crescer o RC até ser o maior clube do mundo!

**Short description (EN):**
Bikes, missions and mates: grow the RC into the biggest club in the world!

**Descrição completa (PT):**
Bem-vindo ao RC Riding Club! Pega na tua 125, cumpre missões para o grupo e transforma o clube no maior clube de motas do mundo.

• Cidade em pixel art vista de cima, com trânsito, polícia, parques e uma floresta com trilhos
• Missões no telemóvel do jogo: entregas, encontros, corridas e muito mais
• Motoqueiros rivais que te desafiam para corridas, cavalinhos e piões
• Mais de 25 motas, de 50cc a 2500cc, com melhorias, pinturas, capacetes, casacos e buzinas
• Grupo do Facebook dentro do jogo, com publicações e novos membros
• O clube cresce sozinho, mesmo quando não estás a jogar
• Licença RC Eats: faz entregas e ganha gorjetas
• Mini-jogos 3D: oficina, bomba de gasolina, café, arrancadas e cavalinhos
• História com 6 capítulos e diálogos divertidos com 3 respostas
• Prémios diários, conquistas e diamantes escondidos pela cidade
• DLC: Lisboa e Porto, Ilha de Man TT e Motas Clássicas

Respeito acima de tudo. Capacete sempre.

**Full description (EN):**
Welcome to RC Riding Club! Grab your 125, complete missions for the crew and turn the club into the biggest motorcycle club in the world.

• Top-down pixel-art city with traffic, police, parks and a forest with dirt trails
• Missions on your in-game phone: deliveries, meet-ups, races and more
• Rival riders who challenge you to races, wheelies and donuts
• 25+ bikes from 50cc to 2500cc, with upgrades, paints, helmets, jackets and horns
• An in-game Facebook-style group with posts and new members
• Your club keeps growing even when you're not playing
• RC Eats licence: do deliveries and earn tips
• 3D mini-games: workshop, petrol pump, coffee, drag races and wheelies
• 6-chapter story with funny 3-choice dialogues
• Daily rewards, achievements and diamonds hidden around town
• DLC: Lisbon and Porto, Isle of Man TT and Classic Bikes

Respect above all. Helmets always.

**Categoria:** Jogos → Corridas
**Política de privacidade:** https://bushiannms.github.io/rc-riding-club/privacy.html
**Imagens:** usa as capas que já tens (1920×1080) e capturas de ecrã do telemóvel.

## 2. Produtos para criar (Monetizar → Produtos)

| ID do produto | Tipo | Preço |
|---|---|---|
| gems_100 | Produto in-app (consumível) | 0,99 € |
| gems_550 | Produto in-app (consumível) | 4,99 € |
| gems_1200 | Produto in-app (consumível) | 9,99 € |
| gems_2600 | Produto in-app (consumível) | 19,99 € |
| noads | Produto in-app (não consumível) | 2,99 € |
| dlc_portugal | Produto in-app (não consumível) | 4,99 € |
| dlc_ilha | Produto in-app (não consumível) | 3,99 € |
| dlc_classicas | Produto in-app (não consumível) | 2,99 € |

Os IDs têm de ficar exatamente assim.

## 3. Segurança dos dados (questionário da Play Console)
- Recolhe dados? Sim, só através do AdMob (identificador de publicidade, dados de utilização e diagnóstico).
- Partilha dados? Sim, com a Google (publicidade).
- Dados encriptados em trânsito? Sim.
- O utilizador pode pedir para apagar? Sim (apagar save ou desinstalar).
- Compras: processadas pelo Google Play.

## 4. Classificação de conteúdo
- Violência: não (as colisões não ferem pessoas de forma gráfica).
- Jogos de sorte com dinheiro real: os jogos da sorte usam diamantes (que podem ser comprados). Responde "Sim, compras com elementos aleatórios" e indica que as probabilidades estão visíveis.
- Compras na app: sim. Anúncios: sim.

## 5. Chave de assinatura (uma vez só)
No GitHub, em Settings → Secrets and variables → Actions → New repository secret, cria:
- `ANDROID_KEYSTORE_B64` → o conteúdo do ficheiro rc-upload.b64.txt
- `ANDROID_KEYSTORE_PASSWORD` → a palavra-passe da chave
- (quando tiveres AdMob) `ADMOB_APP_ID` → o ID da app AdMob (começa por ca-app-pub- e tem um ~)

A partir daí, cada versão gera também o ficheiro `rc-riding-club.aab`, que é o que se envia para a Play Console. Guarda o ficheiro rc-upload.jks num sítio seguro: sem ele não consegues atualizar a app.

## 6. AdMob
1. Cria a conta em admob.google.com e adiciona a app Android "RC Riding Club".
2. Cria dois blocos de anúncios: "Recompensado" e "Intersticial".
3. Envia os dois IDs dos blocos ao Claude para os pôr no jogo, e põe o ID da app no segredo `ADMOB_APP_ID`.

# RC Riding Club

Jogo de motas em pixel art ao estilo GTA 2: uma cidade de Londres com o Tamisa, missões do clube nas cabines telefónicas, polícia, corridas contra os Big Bikes Only, garagem com 19 motas (de 125cc a 2458cc, marcas fictícias) e mini-jogos 3D (oficina, bombas, café e arrancada).

## Onde está cada coisa
- **Jogo:** `www/index.html` + `www/three.min.js`.
- **Jogar no browser:** com o GitHub Pages ativo (Settings → Pages → Source: GitHub Actions), cada alteração no `main` publica o jogo.
- **APK Android de teste:** cada alteração no `main` publica o APK em **Releases**. Link direto: https://github.com/Bushiannms/rc-riding-club/releases/latest/download/rc-riding-club.apk
- **CrazyGames:** **Actions → Pacote CrazyGames** gera o ZIP com o SDK v3 de anúncios.
- **Versão final Android** (AdMob e compras no Google Play): [`ANDROID.md`](ANDROID.md).

## Monetização
- Anúncios com recompensa opcionais: duplicar o pagamento da missão, reparar a mota, atestar o depósito, limpar as estrelas da polícia e duplicar o prémio diário.
- Anúncios intercalares só entre missões ou à saída de mini-jogos, no máximo 1 a cada 3 minutos. Nunca durante a condução.
- Compras cosméticas (Android): pinturas especiais, capacetes, casacos do clube e Pack Lenda.
- Merch: em `www/index.html`, preenche `merchUrl` em `const CFG=` com o site da loja do clube.

Fora da CrazyGames e sem os plugins Android, os anúncios e as compras funcionam em modo de demonstração.

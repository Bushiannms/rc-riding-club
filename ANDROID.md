# RC Riding Club: versão Android (Capacitor)

O jogo está na pasta `www`. Este repositório já compila um APK de teste automaticamente; estes passos são para a versão final com anúncios e compras. Os anúncios e as compras ligam-se sozinhos quando os plugins existem.

## 1. Criar o projeto
```
npm init -y
npm install @capacitor/core @capacitor/cli @capacitor/android
npx cap init "RC Riding Club" com.rcridingclub.jogo --web-dir www
npx cap add android
```

## 2. Anúncios (AdMob)
```
npm install @capacitor-community/admob
```
- No `index.html`, procura `const CFG=` e troca os IDs de teste da Google (`ca-app-pub-3940256099942544/...`) pelos teus IDs de anúncio com recompensa e de intercalar.
- Junta o teu App ID do AdMob no `AndroidManifest.xml` (meta-data `com.google.android.gms.ads.APPLICATION_ID`).

## 3. Compras (Google Play)
```
npm install cordova-plugin-purchase
```
Cria estes produtos na Play Console (produtos dentro da app):
| SKU | Tipo | Preço sugerido |
|---|---|---|
| pack_pinturas | não consumível | 1,99 € |
| pack_capacetes | não consumível | 0,99 € |
| casacos_rc | não consumível | 0,99 € |
| pack_lenda | consumível | 4,99 € |

Antes de lançar, regista os produtos no arranque (`CdvPurchase.store.register`), chama `store.initialize()` e confirma cada compra no evento `approved` → `verify` → `finish`, como explica a documentação do plugin.

## 4. Merch
Em `const CFG=`, preenche `merchUrl` com o endereço da loja do clube.

## 5. Gerar e testar
```
npx cap sync android
npx cap open android
```
No Android Studio: Build → Generate Signed Bundle (AAB) e carrega-o na Play Console (registo único de 25 USD).

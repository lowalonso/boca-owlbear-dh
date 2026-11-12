# A Boca do Mundo — Extensões pro Owlbear Rodeo

Duas extensões de Daggerheart integradas ao **Dice+**:

| Pasta | Extensão | Pra quem |
|---|---|---|
| `ficha/` | **Ficha dos Quebrados** — os 9 personagens completos e funcionais | jogadores |
| `mestre/` | **Mesa do Mestre** — Medo, Relógio da Fome, bestiário, chefes, party | mestre |

## Como hospedar (GitHub Pages, ~5 min)

1. Crie um repositório **público** no GitHub (ex.: `boca-owlbear`).
2. Suba TODO o conteúdo desta pasta pra raiz do repositório (arraste os arquivos na página do repo → *commit*).
3. No repo: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. Aguarde ~1 min. Seus manifests ficarão em:
   - `https://SEU-USUARIO.github.io/boca-owlbear/ficha/manifest.json`
   - `https://SEU-USUARIO.github.io/boca-owlbear/mestre/manifest.json`

## Instalar no Owlbear

1. Em **owlbear.rodeo → perfil → Extensions → Add Extension**, cole a URL de cada `manifest.json`.
2. Ative as extensões na sala (a Mesa do Mestre só precisa estar ativa pra você; a Ficha, pra todos).

## Configurar o Dice+ (dado azul = Esperança, vermelho = Medo)

1. Instale o **Dice+** (loja de extensões do Owlbear).
2. No Dice+, **Add Dice** e crie:
   - um **d12 azul** chamado `Esperanca`
   - um **d12 vermelho** chamado `Medo`
   - (opcional) um **d6 verde** chamado `Vantagem`
   > Sem acento no nome — a notação referencia o dado pelo nome exato: `1d12{Esperanca}+1d12{Medo}`.
3. Cada jogador que quiser ver os dados 3D com as cores certas cria os seus (ou receba os dados compartilhados pelo Dice+ → menu ⋮ do dado → *Share*).
4. Nas extensões, ⚙ **Dice+** mostra o status da conexão; os nomes dos dados são configuráveis ali.
   Sem Dice+ instalado tudo continua funcionando com a rolagem interna.

## O que cada uma faz

**Ficha dos Quebrados**
- Escolha 1 dos 9 Quebrados → ficha completa: PV, Fadiga, Armadura, Esperança em pinos clicáveis e editáveis.
- Limiar de dano visível + botão **Sofrer dano** (aplica 1/2/3 PV pelos limiares, com opção de gastar Armadura).
- Clique num **atributo** → rola a dualidade (normal/vantagem/desvantagem) no Dice+.
  - **Com Esperança** → +1 Esperança automático.
  - **Com Medo** → +1 no Medo do Mestre e aviso pra todos: *"A Boca salivou X vezes…"*.
  - **Crítico** (dados iguais) → +1 Esperança e recupera 1 Fadiga; dano de arma ganha +máximo.
- Clique numa **arma** → ataque + dano numa rolagem só (dualidade + dados de dano do patamar).
- **Experiências**: usar desconta 1 Esperança, arma +N na próxima rolagem e mostra uma carta pra todos.
- **Cartas de domínio** com texto completo + botão *mostrar a todos*.
- Contador de **Medo** e **Fome** sempre no topo (e badge vermelho no ícone da extensão).

**Mesa do Mestre**
- **Medo** gigante (+/−) alimentado automaticamente pelas fichas; **banner flutuante no topo** da tela de todos (liga/desliga).
- **Relógio da Fome** (6 segmentos) sincronizado.
- **Bestiário** (8 inimigos) e **12 Chefes** com ataques clicáveis (d20 de ataque, dados de dano), fases, estratégia e a revelação de lore (com botão de mostrar a todos ao vencer).
- **Party ao vivo**: PV/Fadiga/Armadura/Esperança de cada jogador conectado.
- Alvo das rolagens: **todos veem** ou **só o Mestre**.

## Testar sem o Owlbear

Abra `ficha/index.html` ou `mestre/index.html` direto no navegador: entra em **modo demonstração** (tudo clicável, rolagem interna).

# Operação Código 0 — Fim dos Tempos

Continuação em HTML/Three.js do shooter enviado. A campanha nova tem três atos ambientados no México e no complexo da bomba; os modos originais de coop local, versus e zumbis, além de armas, controles, HUD, texturas retrô e opções, continuam disponíveis.

## Abrir e jogar

Abra `index.html` em um navegador moderno. O Three.js r128 está incluído localmente no repositório, então o motor 3D não depende de um CDN para iniciar. No menu, escolha **História Solo** ou **História 2 Players** para iniciar o briefing. Para uma dupla local, o jogador 1 usa teclado e mouse; o jogador 2 usa um controle conectado.

### Controles

- **P1:** WASD mover, mouse mirar, botão esquerdo atirar, botão direito mirar, Shift correr, Espaço pular, R recarregar, Q ou roda trocar arma, E pegar arma, F interagir, Esc pausar.
- **P2/controle:** analógico esquerdo mover, analógico direito mirar, RT atirar, LT mirar, X recarregar, A pular, RB trocar arma, B pegar arma, Y interagir/lanterna nos zumbis, LB/L3 correr, Start pausar.
- **Zumbis:** F liga/desliga a lanterna; na campanha, F interage com alvos e objetivos.

## Campanha — três atos

1. **México / captura:** briefing de rádio; inserção na cidade, encontro com a equipe local, combate e coleta de três documentos. No edifício, reduza a saúde do chefe e pressione **F** perto dele para capturá-lo vivo.
2. **Interrogatório / coordenadas:** a equipe obtém do chefe a localização da bomba e a senha **SIERRA-09**; elimine a escolta e recupere a pasta criptografada.
3. **Infiltração / desativação:** aproxime-se dos guardas e pressione **F** para neutralizá-los em silêncio. O primeiro abate concede o disfarce; acesse o terminal, enfrente os reforços e desarme a bomba com a senha indicada. Depois da queda do protagonista, a perspectiva passa ao parceiro; chegue ao memorial e pressione **F** no caixão para prestar respeito.

## Falas e direção de voz

As falas principais são gravações compactas em MP3, armazenadas em `voz/` e carregadas sob demanda durante o briefing e as cutscenes; isso evita baixar os áudios no carregamento inicial do jogo. Se um clipe não puder tocar, a síntese de voz em português brasileiro do navegador é usada como fallback. As legendas permanecem disponíveis.

| Personagem | Direção de voz |
|---|---|
| SGT. SILVA | Voz masculina adulta, grave, firme e econômica. Rádio baixo, autoridade sem gritar; em aproximação, quase sussurro. Nas ordens de combate, dicção curta e incisiva. |
| CB. GOMES | Voz masculina média, calma e prática. Tom de cobertura, frases rápidas; tensão contida durante o tiroteio. |
| SD. REIS | Voz mais jovem, clara e atenta. Baixo volume nas instruções de infiltração; firme ao comunicar contato e o código. |
| COMANDO | Voz neutra de rádio, formal, seca e distante. |

### Roteiro da abertura

1. **SGT. SILVA:** “Equipe Alfa, os documentos recolhidos revelam uma base dos cartéis no México. Há indícios de uma bomba nuclear em construção.” — tom grave, baixo, confidencial.
2. **CB. GOMES:** “Eles querem lançá-la contra os Estados Unidos. Uma guerra abriria caminho para expandirem o tráfico e dominarem outros países.” — preocupação controlada, sem dramatizar.
3. **SD. REIS:** “Precisamos capturar o chefe vivo. Ele vai confirmar o local exato e revelar a senha de desativação.” — sussurro atento, objetivo.
4. **SGT. SILVA:** “Peguem o equipamento. Vamos descer na cidade, reunir a equipe local e encontrá-lo. Ninguém dispara antes da hora.” — ordem curta, autoridade tranquila.

As falas seguintes cobrem a inserção, a captura, as coordenadas, o disfarce, os reforços, a senha, a queda do protagonista e o memorial; as cenas de extração, interrogatório, infiltração, desarme e velório usam arquivos MP3 em `voz/`.

## Efeitos sonoros

Os efeitos também ficam no repositório, em `sfx/`, e são carregados junto do jogo: cada uma das oito armas (M4, AK-47, UMP, MP5, pistola, escopeta, revólver e sniper) tem um disparo próprio. Há ainda sons de fuzil inimigo, impacto em inimigos, dano recebido pelo jogador, esforço ao erguer o sargento e vocalizações de zumbi para gemido, ataque e derrota.

## Publicação

O repositório conectado é público. O GitHub Pages ainda não está habilitado neste repositório; para testar sem Pages, abra `index.html` ou use um servidor estático. Os arquivos de áudio ficam na pasta `voz/` e devem ser mantidos junto do HTML para que as falas gravadas sejam encontradas.

# Versão Brasileira

Tradução do conteúdo dos jogos, Red, Blue e Yellow.
A ripagem foi feita a partir da versão Vermelha, como Blue usa os mesmos textos não é afetada, porém Yellow apresenta algumas inconsistências no diálogo.

O processo de ripagem não foi perfeito e alguns texto podem estar completamente errados ou quebrados.
Alguns NPCs estão falando frases de outros próximo deles. Alguns golpes podem dar descrição de outro golpe.
Algumas coisas do recomp foram reconstruídas do zero e a tradução não pega, ficando em Inglês por enquanto (ex: Cassino).
Versão Amarela não é 100% suportada por apresentar os diálogos padrões para Red/Blue.


Qualquer erro ou inconsistência encontrada podem reportar que irei atualizar o patch assim que possível corrigir para deixar os 3 jogos 100%.

OBS: Mods adicionais ao recomp não são suportados, apesar de usar algumas labels iguais se serem traduzidos parcialmente, esse patch aqui é apenas para o conteúdo original do jogo.

# Trechos sem traduzir por incompatibilidade do recomp (serão corridigos automaticamente atualizando o recom e não a tradução:
- JOGADOR got a MAGIKARP! //No centro da Mt.Lua
- Ao vencer a liga, o Professor Carvalho não fala o nome do seu inicial.
- Game Corner Cassino foi todo refeito do zero e não usa textos normais da rom.
- WITHDRAW/DEPOSIT no PC.

# Opções Extra do Menu do Mod
- Desativar a traduções dos Golpes (reverte para Inglês);
- Reativar a exibição de "Pokémon Inimigo" e o "usou" na linha de baixo junto com o golpe. É necessário apenas se for usar a U.I. original do jogo, praticamente todos os mods de aparência permitem exibir mais que 18 caracteres por linha;
- Quebra de linha no inventário. Recomp vanilla deixa os valores na mesma linha, algo que só é compatível com itens de no máximo 12 caracteres, como os traduzidos usam até 17 foi necessário abaixar. Desligue se algum mod conflitar;
- Trainer Card. Fiz as correções necessárias para traduzir corretamente e adicionei essa opção para desligar e voltar ao padrão (não traduz MONEY e TIME).


# Originaly forked from:
### VersãoVermelha

Brazilian Portuguese, ripped from the **Hyd~Traduções Pokémon Versão
### Vermelha v1.3.1** IPS patch rather than translated by hand.
Generated with `python3 tools/modkit.py translation versaovermelha`, then filled
by rom hack exports.

2796 strings register at boot. Everything unfilled falls through to
English, so this is playable at every point along the way.
Some missing wont make for a terrible experience, and itll do for now!
#### What is not translated, and why

**138 dialogue lines.** Label recovery follows `TX_FAR` records out of map
scripts. A few labels are reached another way and have no recoverable
counterpart; a few more decode to bytes the port's text model cannot
represent.

##### Layout
- `manifest.json` - identity and the engine version range
- `main.lua` - registers whatever is filled in and skips whatever is not
- `lang/` - the catalogs
- `assets/font/latin.png` - the accented glyph page, base `0x100`
- `overrides/` - any obvious sprite diffs

# Normalização passo a passo

**▶ Acesse:** https://cidandrade.github.io/normalizacao/

Página interativa para entender a **normalização** de um banco de dados, da planilha bagunçada até a 3FN. O caso é a ficha de pedidos da Papelaria Ponto Final, que traz de propósito um atributo composto (endereço), um multivalorado (telefones), um grupo repetitivo (itens), uma dependência parcial e duas dependências transitivas.

Material da disciplina **Modelagem de Banco de Dados**, do Prof. Cid Andrade (UNICID).

## As etapas

| Etapa | O que tem |
|-------|-----------|
| 0. O caso | A ficha original e as anomalias de inserção, atualização e exclusão. |
| 1. Chaves e dependências | O primeiro passo: chaves candidatas, primárias e alternativas, e o mapa interativo das dependências funcionais (DF1–DF8). |
| 2. 1FN | Atributo composto decomposto no lugar; multivalorado e grupo repetitivo viram tabelas. |
| 3. 2FN | Exame atributo a atributo de `ITEM_PEDIDO` e a saída de `PRODUTO` (dependência parcial). |
| 4. 3FN | As cadeias transitivas viram `CLIENTE` e `VENDEDOR`. |
| 5. Chaves estrangeiras | Diagrama das seis tabelas, de onde veio cada FK e uma verificação de integridade referencial (com simulação de erro). |
| 6. Conferência | Cada tabela em cada forma normal, preservação das dependências, junção que reconstrói a ficha, script SQL e teste rápido. |

Em cada etapa, o botão **Destacar dados repetidos** mostra a redundância que ainda resta. O endereço guarda a etapa (por exemplo, `#fn2`), e as setas ← → do teclado avançam e voltam.

## Arquivos

- `index.html`: a página inteira, num arquivo só. Só busca as Google Fonts de fora.

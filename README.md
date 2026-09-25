# Dashboard Conversão - Pacote R3 GitHub Pages

## Estrutura

- `index.html`: dashboard e conversor atualizado.
- `dados/manifest.json`: relação dos JSONs publicados.
- `.nojekyll`: indica publicação estática no GitHub Pages.

## Padrão dos arquivos

O nome é gerado pela coluna `NR_ANO_MES`:

- `202606` gera `ND-26-06.json` ou `BL-26-06.json`.
- `202607` gera `ND-26-07.json` ou `BL-26-07.json`.

## Fluxo recomendado

1. Abra o `index.html` atualizado.
2. Selecione e processe somente o CSV ND.
3. Confira na mensagem o nome e o tamanho estimado.
4. Baixe o JSON ND.
5. Aguarde a mensagem de memória liberada.
6. Selecione e processe o CSV BL.
7. Baixe o JSON BL.
8. Envie os dois JSONs para a pasta `dados`.
9. Atualize `dados/manifest.json` com os nomes reais.

Exemplo:

```json
{
  "arquivos": [
    "ND-26-06.json",
    "BL-26-06.json"
  ]
}
```

## Publicação

Mantenha `index.html`, `README.md`, `.nojekyll` e a pasta `dados` na raiz da branch configurada no GitHub Pages.

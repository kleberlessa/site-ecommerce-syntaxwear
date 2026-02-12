# Architecture

## Nomenclatura

- Pastas e arquivos: `kebab-case`
- Classes CSS: BEM (`block__element--modifier`)

## CSS (metodologia)

### BEM

- **Block**: componente ou seção independente (`product-card`)
- **Element**: parte interna do block (`product-card__title`)
- **Modifier**: variação de estado/estilo (`product-card--featured`)

Regras:

- Evitar seletores por tag para estilização de componentes.
- Evitar encadeamento profundo (manter baixa especificidade).

## Estrutura de estilos

- `src/styles/tokens/`: design tokens (cores, espaçamentos, tipografia)
- `src/styles/base/`: reset/normalização, tipografia base, helpers globais essenciais
- `src/styles/layout/`: grid, containers, seções macro da página
- `src/styles/components/`: estilos por componente (BEM)
- `src/styles/utilities/`: classes utilitárias (uso consciente)

## Hierarquia de importação de CSS

Ordem recomendada:

1. `tokens/`
2. `base/`
3. `layout/`
4. `components/`
5. `utilities/`

## Separação de responsabilidades

- `src/assets/`: somente arquivos estáticos (imagens, ícones, fontes)
- `src/data/`: dados mockados para simular futuras respostas de API
- `src/utils/`: utilitários (ex.: formatação, mapeamentos) — sem dependência de DOM quando possível
- `src/components/`: componentes reutilizáveis
- `src/layouts/`: composições e estruturas de página
- `src/pages/`: páginas (ex.: `home`)

# Syntaxwear — Home (E-commerce de Sapatos)

Projeto inicial para construção da **Home** de um e-commerce de sapatos, começando em **HTML/CSS (sem JS)**, mas estruturado para evoluir com segurança para uma aplicação mais complexa (API, carrinho, checkout, marketplace multi-vendedor).

## Objetivo

- Entregar uma Home sólida (menu, hero, destaque, grid de produtos, rodapé)
- Manter a base organizada para evolução futura sem retrabalho

## Estrutura de pastas

```
/docs
  architecture.md
/src
  /assets
    /images
    /icons
    /fonts
  /components
  /layouts
  /pages
  /styles
    /base
    /tokens
    /layout
    /components
    /utilities
  /data
  /utils
```

## Convenções

- **Nomenclatura (pastas/arquivos/classes)**: `kebab-case`
- **CSS**: metodologia **BEM**
- **CSS import order**: ver `docs/architecture.md`

## Padrão de commits (Conventional Commits)

Formato:

```
<type>(<scope>): <subject>
```

Tipos comuns:

- `feat`: nova funcionalidade
- `fix`: correção de bug
- `chore`: tarefas internas (configs, tooling)
- `docs`: documentação
- `refactor`: refatoração sem mudar comportamento
- `style`: formatação (sem alterar lógica)
- `test`: testes

Exemplos:

- `chore(repo): add base folder structure`
- `docs(architecture): define css conventions`

## Branching

- Branch principal de trabalho: `develop`
- Branches de feature: `feat/<escopo>-<resumo>`
- Branches de correção: `fix/<escopo>-<resumo>`

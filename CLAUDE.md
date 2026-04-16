# CLAUDE.md — PERFILHUMANORH

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** PERFILHUMANORH
**Nicho:** Negócios e Empreendedorismo
**Keywords:** Nossa historia e criada pela conexao entre pessoas formando relacoes de confianca
**Paleta de cores:** gold | **Fonte:** playfair

Nossa história é criada pela conexão entre pessoas, formando relações de confiança. Foi esse motivo que nos inspirou, desde o começo, a desafiar limites e buscar novas formas para cuidar do ambiente de trabalho e auxiliar pessoas a conseguirem uma oportunidade de emprego. Somos especialistas na área de RH e entregamos conteúdo e conhecimentos para evoluir pessoas e empresas Mesmo nos momentos de incerteza, sempre soubemos que seria possível, porque cada desafio reforçou ainda mais nosso sonho de transformar positivamente as organizações. Ajudamos mais de 3.000 pequenas e médias empresas, como a sua, a crescerem de forma sustentável e pessoas a alcançarem seu tão almejado emprego. Contamos com colunistas que possuem ampla experiência no mercado, temos uma equipe preparada para contribuir com informações e novidades.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-H |
| Hero | Hero-E |
| Features | Features-E |
| About Section | About-F |
| Posts | Posts-C |
| Footer | Footer-H |
| Página Sobre | Sobre-J |
| Página Contato | Contato-J |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```

# Sinal Verde - Site Estático

Este projeto está preparado para GitHub Pages usando URLs sem `.html` nas subpáginas.

## Estrutura de URLs

- Página inicial: `/`
- Blog: `/blog/`
- Sobre nós: `/sobrenos/`
- Política de privacidade: `/privacidade/`
- Termos: `/termos/`
- Cursos: cada curso fica em sua própria pasta, por exemplo `/cursomopp/`

No GitHub Pages, essa estrutura funciona porque cada subpágina possui um `index.html` dentro da pasta correspondente.

## Publicação no GitHub Pages

1. Envie estes arquivos para o repositório.
2. No GitHub, acesse `Settings > Pages`.
3. Em `Build and deployment`, selecione `Deploy from a branch`.
4. Escolha a branch principal e a pasta `/root`.
5. Salve e aguarde a URL pública ser gerada.

O arquivo `.nojekyll` deve permanecer na raiz para o GitHub Pages servir os assets exatamente como estão.

## Recomendações

- O GitHub Pages não executa PHP. O arquivo `assets/inc/sendemail.php` não funcionará nesse ambiente. Para formulários, use um serviço externo como Formspree, FormSubmit, Basin ou um backend próprio.
- A newsletter ainda está sem URL real de integração. Configure o `data-url` do Mailchimp ou remova o bloco de newsletter.
- Assim que o domínio final estiver definido, adicione `canonical`, Open Graph e schema JSON-LD nas páginas principais e nas páginas de curso.
- Mantenha os links internos sem `.html`; use sempre o formato `pagina/`.
- Antes de publicar, teste a navegação por `/blog/`, `/sobrenos/`, `/cursomopp/` e demais cursos.

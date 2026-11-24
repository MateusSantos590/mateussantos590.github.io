# mateussantos590.github.io
Portfólio pessoal de Mateus Telles: suporte em TI, dados e projetos em Python.

Site estático em um único `index.html` (sem build), publicado pelo GitHub Pages.
Versão em inglês: `https://mateussantos590.github.io/?lang=en`

## Como completar o site
- **Currículo:** envie `curriculo.pdf` para a raiz. O botão "Baixar currículo" aparece sozinho.
- **Foto:** envie `foto.jpg` (retrato 4:5) para a raiz. Ela substitui o monograma na seção Sobre.
- **Textos em inglês:** ficam no objeto `EN` dentro do `<script>` no fim do `index.html`.

## Segurança
O `index.html` tem uma Content-Security-Policy que só permite os scripts inline cujo hash está na política.
Se editar qualquer `<script>`, recalcule os hashes (sha256 em base64 do conteúdo do script) e atualize `script-src`, senão o script é bloqueado.

# mateussantos590.github.io
Portfólio pessoal de Mateus Telles: suporte em TI, dados e projetos em Python.

Site estático em um único `index.html` (sem build), publicado pelo GitHub Pages.
Versão em inglês: `https://mateussantos590.github.io/?lang=en`

## Como completar o site
- **Currículo:** `curriculo.pdf` é a versão pública, sem telefone. Para atualizar, substitua o arquivo mantendo o nome.
- **Foto:** `foto.jpg` (880x1100, 4:5, sem metadados). Para trocar, substitua o arquivo mantendo o nome e a proporção.
- **Textos em inglês:** ficam no objeto `EN` dentro do `<script>` no fim do `index.html`.

## Segurança
O `index.html` tem uma Content-Security-Policy que só permite os scripts inline cujo hash está na política.
Se editar qualquer `<script>`, recalcule os hashes (sha256 em base64 do conteúdo do script) e atualize `script-src`, senão o script é bloqueado.

## Desempenho
- Fontes IBM Plex hospedadas em `fonts/` (licença SIL OFL 1.1 em `fonts/OFL.txt`), sem dependência do Google Fonts.
- Efeitos contínuos usam só `transform`/`opacity`; o JavaScript faz no máximo uma atualização visual por quadro, limitada a 60 fps.
- Modo leve automático (`html.lite`): ativado em aparelhos com pouca memória/CPU, com economia de dados ligada ou quando a página mede quadros lentos. Desliga o desfoque do menu, o brilho dos cards e a animação do título.

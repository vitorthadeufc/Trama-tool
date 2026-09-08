# Trama

Gerador de **halftone, gravura, stipple e mosaico** 100% vetorial a partir de qualquer imagem — direto no navegador, sem instalar nada e sem depender do Illustrator para gerar o resultado (o SVG final abre e edita normalmente no Illustrator, Figma, Inkscape etc.).

Ferramenta pessoal, inspirada na ideia por trás de plugins de halftone para Illustrator (como o Half Line, da Topia Supply), mas escrita do zero como uma página HTML independente — sem código, ativos ou marca de terceiros.

## Como usar

Não precisa de servidor, build ou instalação: é um único arquivo HTML.

- **Direto do disco**: dê duplo clique em `index.html` (abre no navegador padrão).
- **Publicado (GitHub Pages)**: se o repositório tiver o Pages ativado, acesse a URL que o GitHub gerar (ver abaixo).

## Funcionalidades

- **4 modos**: Meio-tom (halftone AM clássico), Gravura (com três padrões — Retas, com contra-trama/crosshatch; Circular, anéis concêntricos a partir do centro; e Ondulada, linhas com amplitude/frequência ajustáveis), Stipple (pontos aleatórios ponderados por tom) e Mosaico (grade de blocos, com opção de usar as cores originais da imagem).
- **5 formas embutidas** para o Meio-tom e o Stipple: círculo, quadrado, losango, triângulo e cruz.
- **Biblioteca de texturas**: envie seus próprios arquivos `.svg` e use-os como a unidade repetida da trama, no lugar das formas padrão — tingidos automaticamente com a cor da tinta (ou, no mosaico, com a cor de cada célula da imagem).
- Controles de densidade da trama (até 450 células), ângulo, tamanho, ponto preto/branco (levels), inversão de tons, cor da tinta e do papel, fundo transparente.
- Exporta o resultado como **SVG vetorial real** (não é raster disfarçado) — botão de salvar ou copiar o código.
- Imagem de exemplo gerada por código ao abrir, para já mostrar o efeito antes de você enviar a sua.

## Publicar no GitHub

Este projeto não tem nenhuma dependência ou etapa de build — são só arquivos estáticos. Duas formas de colocar no GitHub:

### Sem instalar nada (upload pelo navegador)

1. Crie um repositório novo em [github.com/new](https://github.com/new).
2. Na página do repositório recém-criado, clique em **uploading an existing file** (ou **Add file → Upload files**).
3. Arraste os arquivos desta pasta (`index.html`, `README.md`, `LICENSE`) e clique em **Commit changes**.

### Com Git instalado

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
```

### Ativar o GitHub Pages (para ter um link público da ferramenta)

No repositório: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**. Depois de alguns minutos, a ferramenta fica disponível em `https://SEU-USUARIO.github.io/SEU-REPOSITORIO/`.

## Licença

MIT — veja [LICENSE](LICENSE). Uso livre, inclusive comercial; só mantenha o aviso de copyright.

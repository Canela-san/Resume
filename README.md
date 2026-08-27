# Resume

Repositório com o meu currículo em diferentes formatos, todos escritos em LaTeX. Duas versões estão disponíveis: uma geral, voltada para leitura por sistemas de triagem automática (ATS), e uma versão mais visual, para envio direto ou impressão.

## Como compilar o Currículo Moderno (`cv_moderno.tex`)

Este modelo usa fontes nativas do sistema (Lato e Montserrat) e alguns elementos visuais mais elaborados. Para evitar erros de pacotes ausentes, o caminho mais simples é instalar o ambiente TeX completo, mesmo que isso exija mais espaço em disco.

### 1. Preparação da imagem

Antes de compilar, crie uma pasta `assets` no mesmo diretório do `.tex` e coloque nela uma foto de rosto quadrada (mínimo 800x800px), nomeada exatamente `foto_perfil.png`.

### 2. Instalação das dependências

**Linux (Pop!_OS / Ubuntu):**

```bash
sudo apt update
sudo apt install texlive-full fonts-lato fonts-montserrat
```

**Windows:**

Instale o [TeX Live](https://tug.org/texlive/) completo (ou o MikTeX completo). As fontes [Lato](https://fonts.google.com/specimen/Lato) e [Montserrat](https://fonts.google.com/specimen/Montserrat) precisam ser baixadas e instaladas manualmente — clique com o botão direito no `.ttf` e escolha "Instalar para todos os usuários".

### 3. Compilação

É necessário usar o motor **XeLaTeX**, por causa da renderização das fontes do sistema. O arquivo também precisa ser compilado **duas vezes seguidas**, para que a sidebar, o recorte da foto e as cores de fundo fiquem alinhados corretamente.

```bash
xelatex cv_moderno.tex
xelatex cv_moderno.tex
```

O `cv_moderno.pdf` gerado já sai pronto para uso.

## Exemplos

<table>
<tr>
<th align="center">Currículo Geral (ATS)</th>
<th align="center">Currículo Moderno</th>
</tr>
<tr>
<td align="center" valign="top">
<img src="Geral/Compativel_ATS/img1.png" width="100%" alt="Currículo Geral - Página 1"><br>
<img src="Geral/Compativel_ATS/img2.png" width="100%" alt="Currículo Geral - Página 2"><br>
<img src="Geral/Compativel_ATS/img3.png" width="100%" alt="Currículo Geral - Página 3"><br>
<img src="Geral/Compativel_ATS/img4.png" width="100%" alt="Currículo Geral - Página 4">
</td>
<td align="center" valign="top">
<img src="Geral/Currículo Estiloso/assets/cv_moderno_preview-1.png" width="100%" alt="Currículo Moderno - Página 1"><br>
<img src="Geral/Currículo Estiloso/assets/cv_moderno_preview-2.png" width="100%" alt="Currículo Moderno - Página 2">
</td>
</tr>
</table>
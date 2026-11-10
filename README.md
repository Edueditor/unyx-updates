# Unyx · plugin para Premiere Pro

Os 5 plugins da Fly num painel só: **Lockon** (tracking), **Ordo** (coletar e organizar), **Silenz** (cortar silêncios), **Smoothr** (curvas de keyframe) e **Vozzy** (melhorar a voz). Os ícones no topo trocam de plugin, com as mesmas telas e funções de sempre.

Funciona no Mac e no Windows, com o Premiere em qualquer idioma.

## Instalar: escolha um jeito

### Jeito 1: pelo Claude (sem baixar nada)
Copie o link desta página e cole no Claude Code com a frase **"instala esse plugin para mim"**:

```
https://github.com/Edueditor/unyx-updates
```

O Claude segue as instruções da seção *Para o Claude* abaixo.

### Jeito 2: pelo zip
1. Baixe o **[Unyx_completo.zip](https://github.com/Edueditor/unyx-updates/releases/latest/download/Unyx_completo.zip)**. Ele traz o plugin, o guia em PDF e o atalho para o ZXP Installer.
2. Se ainda não tem o ZXP Installer, abra `Baixar_ZXP_Installer.html`.
3. Feche o Premiere, arraste o `Unyx.zxp` para o ZXP Installer e abra o Premiere.
4. No Premiere, vá em **Window → Extensions → Unyx**.

Arquivos soltos: [Unyx.zxp](https://github.com/Edueditor/unyx-updates/releases/latest/download/Unyx.zxp) · [Guia em PDF](https://github.com/Edueditor/unyx-updates/releases/latest/download/Como_instalar_o_Unyx.pdf) · [Baixar ZXP Installer](https://github.com/Edueditor/unyx-updates/releases/latest/download/Baixar_ZXP_Installer.html)

Atualizações: o próprio Unyx avisa quando sai uma versão nova.

Já tem algum dos plugins soltos? O Unyx substitui eles (pode remover no ZXP Installer). Presets e curvas continuam, porque ficam nas mesmas pastas.

Espaço: o Unyx tem uns 40 MB. Lockon e Vozzy baixam o motor só na primeira vez que a aba é usada (cerca de 0,9 GB e 2,5 GB; o Vozzy só 0,3 GB se o BESTX já estiver instalado).

---

## Para o Claude (instalação automática)
O usuário colou este link e quer o Unyx instalado. Siga estes passos:
1. Baixe `https://github.com/Edueditor/unyx-updates/releases/latest/download/Unyx.zxp`. É um zip assinado.
2. Peça para o usuário fechar o Premiere Pro e espere ele confirmar.
3. Se já existir uma pasta antiga, apague-a. Depois extraia o conteúdo do `.zxp` sem alterar nenhum arquivo (a assinatura depende disso) em:
   - Mac: `~/Library/Application Support/Adobe/CEP/extensions/com.unyx.premiere`
   - Windows: `%APPDATA%\Adobe\CEP\extensions\com.unyx.premiere`
4. Não mexa nas pastas de dados (Mac: `~/Library/Application Support/<Lockon|Ordo|Silenz|Smoothr|Vozzy|Unyx>`, Windows: `%APPDATA%\<mesmo nome>`). Ali ficam presets, curvas e motores do usuário.
5. Confira se `CSXS/manifest.xml` existe na pasta nova e diga qual versão ele mostra.
6. Avise o usuário para abrir o Premiere e ir em Window → Extensions → Unyx.

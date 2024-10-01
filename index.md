# Guia de Configuração do Aplicativo SAM - White Label

---

## Índice

1. [Paleta de Cores](#paleta-de-cores)
2. [Tipografia](#tipografia)
3. [Telas Customizáveis](#telas-customizáveis)
   - [Splash Screen](#splash-screen)
   - [Onboarding Screens](#onboarding-screens)
4. [Imagens Personalizáveis](#imagens-personalizáveis)
5. [Marcadores de Mapas](#marcadores-de-mapas)
6. [Animações](#animações)

---

## Paleta de Cores

![Colors](img/colors.svg)

| Color Name | Code |
| :-------------------------------------- | -----------------------: |  
|  colorHeader | 0xFF1D71B8 |
|  colorHeaderDark |  0xFF094F8A | 
|  colorPrimaryDark |  0xFF094F8A | 
|  colorPrimary |  0xFF1D71B8 | 
|  colorPrimaryLight |  0xFF5EA6E3 | 
|  colorPrimaryLighter |  0xFFBCDBF5 | 
|  colorPrimaryLightest |  0xFFEEF5FB | 
|  colorSecondaryDark |  0xFF0C8553 | 
|  colorSecondary |  0xFF13D485 | 
|  colorSecondaryLight |  0xFF5FF1B5 | 
|  colorSecondaryLighter |  0xFFAFF8DA | 
|  colorSecondaryLightest |  0xFFEFFEF8 | 
|  colorTertiaryDark |  0xFF850C07 | 
|  colorTertiary |  0xFFF76E68 | 
|  colorTertiaryLight |  0xFFFAA4A1 | 
|  colorTertiaryLighter |  0xFFFDD2D0 | 
|  colorTertiaryLightest |  0xFFFDF1F1 | 
|  colorBlack |  0xFF000000 | 
|  colorDark1 |  0xFF2B2E30 | 
|  colorDark2 |  0xFF64686B | 
|  colorDark3 |  0xFFA9ADA6 | 
|  colorDark4 |  0xFFCBCFD1 | 
|  colorLight4 |  0xFFDCDDDE | 
|  colorLight3 |  0xFFEAEBEC | 
|  colorLight2 |  0xFFF4F5F5 | 
|  colorLight1 |  0xFFFBFBFB | 
|  colorWhite |  0xFFFFFFFF | 
|  colorSuccess |  0xFF1D9E62 | 
|  colorSuccessLight |  0xFF8ECFB1 | 
|  colorSuccessLightest |  0xFFEBF9F2 | 
|  colorWarning |  0xFFF78706 | 
|  colorWarningLight |  0xFFFCCF9B | 
|  colorWarningLightest |  0xFFFAF2E9 | 
|  colorError |  0xFFDC2839 | 
|  colorErrorLight |  0xFFFDBCC2 | 
|  colorErrorLightest |  0xFFFAEAEB |

---
## Tipografia

![Colors](img/typography.svg)

> A aplicação de fontes com espaçamentos diferentes e/ou escalas diferentes pode causar o mal funcionamento de partes do aplicativo. 

---

## Telas Customizáveis

### Splash Screen

Tela apresentada quando o aplicativo é iniciado. Tem como objetivo proporcionar uma experiência mais agradável enquanto o aplicativo realiza tarefas de inicialização. Ajuda a reforçar a identidade da marca. Tela 100% customizável, inclusive com a possibilidade de rodar animações lottie. 
`(Conforme especificado em Animações)`

### Onboarding Screens

Conjunto de telas que são apresentadas ao usuário no primeiro uso do aplicativo. Seu objetivo é orientar os usuários e destacar as principais funcionalidades. ```* Recomenda-se o uso de no máximo 3 telas de onboarding.```

Essas telas são compostas por 4 elementos customizáveis:

<br>
<u> 1. Background Image </u>

![Background](assets/images/rmtc/onboarding_background.png)

```
! Este background é compartilhado por todas as telas de Onboarding.
- Dimensões: 390x296 pixels
- Formato: PNG
```

<br>
<u> 2. Onboarding Image </u>

![Onboarding](assets/images/rmtc/onboarding1.png)
```
- Dimensões: 328x207 pixels
- Formato: PNG
```

<br><br>
<u> 3. Título Descritivo </u> <br><br>
   Este texto deve ser um título para a funcionalidade.

   > Tipografia utilizada: Title.Heading02.Semibold

<br>
<u> 4. Descrição </u> <br><br> 

Aqui deve ser feita uma descrição sucinta da funcionalidade.

> Tipografia utilizada: Text.Body01.Regular

---

## Imagens Customizáveis

<u> 1. Boas Vindas </u>

![Imagem1](assets/svg/sign_up_welcome.svg)

```
- Dimensões: 361x433 pixels
- Formato: SVG
```

<u> 2.  </u>

![Imagem1](assets/svg/sign_up_welcome.svg)

```
- Dimensões: 361x433 pixels
- Formato: SVG
- Uso
```


## Marcadores de Mapas

<u> 1. Ônibus </u>

![Imagem1](assets/images/rmtc/pin_onibus.png)

```
- Dimensões: 48x48 pixels
- Formato: PNG 
```

<u> 2. Ponto de Parada </u>

![Imagem1](assets/images/rmtc/home_bus_pin.png)

```
- Dimensões: 48x48 pixels
- Formato: PNGG
```

<u> 3. Ponto de Parada Favoritado </u>

![Imagem1](assets/images/rmtc/home_bus_pin_fav.png)

```
- Dimensões: 48x48 pixels
- Formato: PNG
```

<u> 4. Localização do Usuário </u>

![Imagem1](assets/images/rmtc/pin.png)

```
- Dimensões: 48x48 pixels
- Formato: PNG
```

<u> 5. Ponto de Venda/Recarga </u>

![Imagem1](assets/images/common/pin_venda.png)

```
- Dimensões: 48x48 pixels
- Formato: PNG
```
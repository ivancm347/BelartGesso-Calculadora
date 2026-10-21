# BelartGesso Calculadora

Calculadora de materiais, custos e orçamento para obras de **drywall** — paredes e forros. Tudo em um único arquivo HTML, sem instalação e sem backend: é só abrir no navegador e usar.

## ✨ Funcionalidades

### 🧱 Calculadora de Parede
- Entrada por **comprimento × altura** ou **área total (m²)**
- Desconto automático de **vãos** (portas e janelas)
- Configuração de faces com chapa (1 ou 2), espaçamento dos montantes (40/60 cm) e tamanho da chapa
- Materiais calculados: chapas, **guias e montantes em barras de 3 m**, parafusos, fita, massa e banda acústica

### 🏠 Calculadora de Forro F530
- Entrada por **comprimento × largura** ou **área total (m²)**
- Materiais calculados: chapas, **perfil F530 e cantoneira em barras de 3 m**, suspensões, emendas, parafusos, fita e massa

### 🗺️ Medir na Planta
- Suba a **imagem (PNG/JPG)** ou o **PDF do projeto**
- Navegue pelas páginas do PDF e escolha qual medir
- **Calibre a escala** traçando uma linha sobre uma medida conhecida
- **Trace as paredes** por cima da planta e o app soma os comprimentos
- Envie o total direto para a calculadora de parede com um clique

> 📝 A medição é feita por traçado manual sobre a planta — o app não lê as cotas sozinho. Para PDFs é necessária conexão com a internet (o leitor de PDF carrega via CDN).

### 💰 Orçamento
- Tabela editável de **preços unitários** com cálculo automático
- **Mão de obra por m²**, margem/BDI e total geral
- Exporte a lista de materiais em **CSV**
- Copie o orçamento formatado para **WhatsApp**

## 📐 Premissas de cálculo

| Item | Regra |
|---|---|
| Guias | 2 × comprimento (teto + piso), em barras de 3 m — o arredondamento já cobre os recortes (ex.: 4,20 m → 3 barras) |
| Montantes | 1 por posição vertical: `teto(comprimento ÷ espaçamento) + 1` por parede; 1 barra por montante quando a altura ≤ 3 m |
| Perfil F530 | `teto(largura ÷ espaçamento)` linhas × `teto(comprimento ÷ 3)` barras por linha |
| % de perda | Aplicada em chapas, parafusos, fita e massa — **não** nos perfis |

> Estimativas geométricas para levantamento inicial. Confira sempre a modulação, os vãos, os reforços e as especificações do fabricante.

## 🚀 Como usar

1. Baixe o arquivo `calculadora.html` (ou clone este repositório)
2. Abra o arquivo em qualquer navegador moderno (Chrome, Edge, Firefox, Safari)
3. Não precisa de servidor, instalação nem internet (exceto para ler PDFs na aba Planta)

Também funciona bem no **celular** — o layout é responsivo.

## 🛠️ Tecnologia

- Arquivo HTML único, 100% client-side
- Sem dependências para as calculadoras (PDF.js via CDN apenas na leitura de PDFs)
- Sem banco de dados, sem login, sem rastreamento

## 📄 Licença

Uso livre para orçamentos e obras. Adapte como quiser.

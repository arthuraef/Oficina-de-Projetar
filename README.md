# Oficina de Projetar

Clone estático e responsivo do site [Oficina de Projetar](https://www.oficinadeprojetar.com.br/), enriquecido com melhorias de usabilidade, SEO semântico, independência total de assets e painel administrativo headless integrado via **Sveltia CMS**.

---

## 🌐 Links Principais

- **Site no ar (GitHub Pages):** 👉 **[https://arthuraef.github.io/Oficina-de-Projetar/](https://arthuraef.github.io/Oficina-de-Projetar/)**
- **Painel Administrativo (Sveltia CMS):** 👉 **[https://arthuraef.github.io/Oficina-de-Projetar/admin/](https://arthuraef.github.io/Oficina-de-Projetar/admin/)**
- **Repositório GitHub:** [https://github.com/arthuraef/Oficina-de-Projetar](https://github.com/arthuraef/Oficina-de-Projetar)

---

## ✨ Melhorias Implementadas

### 1. Trama Arquitetônica Infinita (`#svg1772196879_8678`)
- O padrão geométrico no Hero e no rodapé agora se multiplica horizontalmente (`repeat-x` via Flexbox e cálculo dinâmico de viewport) para cobrir 100% da tela em qualquer resolução (de mobile a monitores 4K/Ultrawide), eliminando gaps vazios.

### 2. Conversão & Usabilidade no Rodapé (CRO)
- **E-mail clicável:** `mailto:oficinadeprojetar@gmail.com`
- **Telefone clicável:** `tel:+5581994650330` para ligação direta em celulares.
- **Endereço com Google Maps:** Clique no endereço físico abre rota diretamente no Google Maps.
- **WhatsApp com Mensagens Contextuais:** Cada botão de CTA direciona ao WhatsApp com mensagem personalizada para facilitar o início da conversa.

### 3. SEO Semântico e Acessibilidade (WCAG)
- Títulos reestruturados com tags semânticas `<h1>`, `<h2>` e `<h3>` mantendo a estética visual original intacta.
- Atributos `alt` descritivos adicionados em todas as imagens e ícones para leitores de tela e Google Imagens.

### 4. Correção da Imagem de Fundo do Rodapé
- A imagem de padrão geométrico no rodapé (`MfjCEzXdXf5u2rniemAvj53tU6Y.png`) utilizava `object-fit: fill` no desktop, o que causava distorção e achatamento. Foi corrigida para `object-fit: cover; object-position: center;`, mantendo nitidez e proporções exatas.

### 5. Independência Total de Assets
- Todos os 29 arquivos visuais (PNGs, JPEGs, SVGs) e o vídeo institucional (`.mp4`) foram baixados e salvos localmente em `assets/images/` e `assets/videos/`.
- O vídeo institucional conta agora com imagem de capa (`poster`) e `preload="metadata"`, eliminando o quadro preto vazio anterior.

---

## 🎛️ Painel de Conteúdo (Sveltia CMS)

O projeto conta com o **Sveltia CMS** integrado em [`/admin/`](https://arthuraef.github.io/Oficina-de-Projetar/admin/).

Ele permite que você edite os textos e imagens do site de forma visual diretamente pelo navegador:
- **Configurações Gerais:** E-mail, telefone, endereço, links de redes e mensagens de WhatsApp.
- **Hero:** Título principal, subtítulo e imagem de abertura.
- **Manifesto & Valores:** Textos institucionais e render ilustrativo.
- **Tipologias & Especialidades:** Lista de soluções sob medida.
- **Vídeo Institucional:** Chamadas e arquivos de mídia.
- **Metodologia:** As 4 etapas do projeto (*Mergulho, Afinação, Desenho executivo, Acompanhamento*).

### Como Acessar o CMS:
1. Abra `https://arthuraef.github.io/Oficina-de-Projetar/admin/` (ou `http://localhost:8000/admin/` localmente).
2. Conecte-se com sua conta GitHub ou utilize a opção **"Trabalhar com Repositório Local"** para editar sem precisar logar.
3. Ao salvar qualquer alteração, o Sveltia CMS grava automaticamente um commit no repositório, disparando a atualização do site.

---

## 🚀 Como Executar Localmente

```bash
git clone https://github.com/arthuraef/Oficina-de-Projetar.git
cd Oficina-de-Projetar
python3 -m http.server 8000
# Acesse o site em http://localhost:8000
# Acesse o CMS em http://localhost:8000/admin/
```

---

© Oficina de Projetar. Todos os direitos reservados.

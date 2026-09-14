# Landing Page — Dra. Mylene Nagato

Landing page institucional desenvolvida para apresentar a clínica e o trabalho da **Dra. Mylene Nagato**, médica especialista em dor, com foco em dores crônicas e abordagem integrada de cuidado.

O projeto foi construído a partir dos materiais de divulgação fornecidos pela clínica, reaproveitando a identidade visual, a paleta de cores, os principais textos institucionais e as informações de contato presentes nos panfletos.

## Objetivo do projeto

Criar uma presença digital simples, profissional e responsiva para a clínica, permitindo que pacientes encontrem rapidamente informações sobre:

- a médica e sua abordagem de atendimento;
- dor crônica e fatores associados;
- tratamentos e possibilidades de cuidado;
- localização do consultório;
- telefone e WhatsApp;
- redes sociais;
- chamada para agendamento de consulta.

## Tecnologias utilizadas

- **HTML5** — estrutura e conteúdo da página;
- **CSS3** — identidade visual, responsividade e animações de interface;
- **JavaScript** — menu responsivo e atualização automática do ano no rodapé;
- **Google Fonts** — Montserrat e Playfair Display.

Não há dependências, frameworks ou processo de build. O projeto pode ser aberto diretamente no navegador.

## Estrutura de arquivos

```text
landing_clinica_mylene/
├── index.html
├── style.css
├── script.js
└── README.md
```

## Identidade visual

A interface foi inspirada diretamente nos panfletos da clínica.

### Cores principais

- azul institucional — utilizado em títulos, botões e seções de destaque;
- azul claro — utilizado em fundos e áreas de acolhimento;
- branco — base do conteúdo e contraste;
- amarelo — utilizado pontualmente como destaque visual;
- verde/mint — utilizado como cor complementar.

As cores estão centralizadas em variáveis CSS no início do arquivo `style.css`, facilitando futuras alterações.

```css
:root {
  --navy: #0f4a8c;
  --sky-soft: #eef6fb;
  --yellow: #f0c221;
  --mint: #9ee9ce;
}
```

## Seções implementadas

A página contém:

1. **Header com navegação fixa**
2. **Hero / apresentação principal**
3. **Sobre o atendimento**
4. **Explicação sobre dor crônica**
5. **Fatores relacionados à dor crônica**
6. **Tratamentos e possibilidades de cuidado**
7. **Apresentação da Dra. Mylene Nagato**
8. **Redes sociais**
9. **Contato e localização**
10. **CTA final para agendamento**
11. **Botão flutuante do WhatsApp**
12. **Rodapé institucional**

## Informações já configuradas

### WhatsApp

```text
(11) 95900-7084
```

O botão utiliza o link direto do WhatsApp com uma mensagem inicial de solicitação de consulta.

### Instagram

```text
@dramylenenagato
```

### Endereço

```text
Rua Estela, 515
Vila Mariana — São Paulo/SP
Bloco F — Conjunto 51
```

> Antes da publicação oficial, confirme com a clínica o endereço completo e a forma exata como ele deve ser divulgado.

## Conteúdos que ainda devem ser preenchidos

Alguns elementos foram mantidos propositalmente como templates porque as informações não estavam disponíveis nos materiais enviados.

### Foto da médica

No `index.html`, procure por:

```text
INSERIR FOTO PROFISSIONAL DA DRA. MYLENE AQUI
```

ou

```text
COLOCAR FOTO DA DRA. MYLENE AQUI
```

Sugestão: utilizar uma fotografia profissional em formato vertical, com boa iluminação e fundo neutro ou no próprio consultório.

### Formação e credenciais

Adicionar ou validar:

- CRM;
- RQE, quando aplicável;
- especialidades registradas;
- formação acadêmica;
- cursos e pós-graduações;
- experiência profissional;
- instituições de formação;
- breve biografia profissional.

### Informações da clínica

Também é recomendado completar:

- horário de funcionamento;
- e-mail;
- formas de pagamento;
- convênios ou informação de atendimento particular;
- acessibilidade;
- estacionamento;
- política de agendamento e cancelamento;
- telefone fixo, se utilizado;
- mapa incorporado do Google Maps.

### QR Code

Há um espaço reservado para o QR Code das redes sociais. Substitua o placeholder pela imagem oficial utilizada pela clínica.

## Como executar localmente

### Opção 1 — abrir diretamente

Abra o arquivo:

```text
index.html
```

no navegador.

### Opção 2 — usando VS Code + Live Server

1. Abra a pasta no **Visual Studio Code**.
2. Instale a extensão **Live Server**.
3. Clique com o botão direito em `index.html`.
4. Selecione **Open with Live Server**.

O site será aberto em um endereço semelhante a:

```text
http://127.0.0.1:5500
```

### Opção 3 — servidor local com Python

Dentro da pasta do projeto:

```bash
python -m http.server 8000
```

Depois acesse:

```text
http://localhost:8000
```

## Como alterar o número do WhatsApp

No `index.html`, procure por:

```text
5511959007084
```

O formato usado pelo WhatsApp deve conter:

```text
55 + DDD + telefone
```

Exemplo:

```html
<a href="https://wa.me/5511959007084">Falar pelo WhatsApp</a>
```

## Como trocar as fotos

Uma forma recomendada é criar a pasta:

```text
assets/images/
```

Exemplo:

```text
assets/
└── images/
    ├── dra-mylene.jpg
    ├── consultorio.jpg
    └── logo.png
```

Depois substitua o placeholder no HTML por algo como:

```html
<img
  src="assets/images/dra-mylene.jpg"
  alt="Dra. Mylene Nagato"
  class="doctor-image"
/>
```

## Como incorporar o Google Maps

Substitua a área `.map-placeholder` por um `iframe` fornecido pelo Google Maps.

Fluxo sugerido:

1. Pesquise o endereço no Google Maps;
2. clique em **Compartilhar**;
3. escolha **Incorporar um mapa**;
4. copie o `iframe`;
5. substitua o placeholder correspondente no `index.html`.

## Responsividade

A landing page foi estruturada para funcionar em:

- desktop;
- notebooks;
- tablets;
- smartphones.

O menu principal é convertido automaticamente em menu mobile em telas menores.

## SEO básico

O projeto já contém:

- `lang="pt-BR"`;
- `meta viewport`;
- título da página;
- meta description;
- estrutura semântica com `header`, `main`, `section`, `article`, `nav` e `footer`;
- textos alternativos ou indicações para imagens.

Para uma versão de produção, também é recomendado adicionar:

- favicon;
- Open Graph (`og:title`, `og:image`, etc.);
- Schema.org para `Physician` / `MedicalClinic`;
- Google Search Console;
- Google Analytics ou ferramenta equivalente, caso aprovado pela clínica;
- otimização das imagens em WebP/AVIF.

## Deploy

Por ser um projeto estático, pode ser publicado facilmente em serviços como:

- GitHub Pages;
- Vercel;
- Netlify;
- Cloudflare Pages;
- hospedagem convencional via FTP/cPanel.

### GitHub Pages

Depois de enviar o projeto para um repositório GitHub:

1. acesse **Settings**;
2. abra **Pages**;
3. em **Build and deployment**, selecione a branch principal;
4. salve;
5. aguarde a URL pública ser gerada.

## Melhorias futuras sugeridas

Para uma próxima versão, podem ser implementados:

- formulário de contato com backend;
- integração com agenda online;
- botão de agendamento por Doctoralia ou outra plataforma;
- mapa real do consultório;
- seção de dúvidas frequentes;
- depoimentos, desde que autorizados e adequados às normas aplicáveis;
- blog ou seção de conteúdos educativos;
- painel simples para editar textos sem alterar código;
- otimização de SEO local;
- animações leves durante o scroll;
- integração com CMS, como WordPress, Sanity ou Strapi.

## Atenção sobre conteúdo médico

Os textos da página foram construídos com base nos materiais promocionais disponibilizados para o desenvolvimento e incluem alguns campos temporários.

**Antes da publicação oficial**, todo conteúdo relacionado a:

- especialidades;
- títulos profissionais;
- tratamentos;
- procedimentos;
- benefícios terapêuticos;
- indicações clínicas;
- formação e credenciais;

 deve ser revisado e aprovado pela médica responsável.

Também é recomendado revisar a versão final de acordo com as normas vigentes do **Conselho Federal de Medicina (CFM)** e do **Conselho Regional de Medicina (CRM)** referentes à publicidade médica.

## Observação

Este projeto é uma primeira versão de uma landing page institucional. A arquitetura foi mantida propositalmente simples para facilitar manutenção, personalização e publicação.

---

**Projeto:** Landing Page — Dra. Mylene Nagato  
**Tipo:** Site institucional / Landing Page  
**Stack:** HTML, CSS e JavaScript  
**Idioma:** Português — Brasil

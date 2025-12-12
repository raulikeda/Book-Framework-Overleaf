# Template de Livro (LaTeX + Overleaf)

Este repositório fornece um template organizado e estável para escrita de livros em LaTeX, pensado para funcionar de forma integrada com **Overleaf**.

Ele foi criado para textos longos, técnicos ou acadêmicos, nos quais organização, manutenção ao longo do tempo e versionamento são tão importantes quanto o conteúdo em si.

---

## Para que este template foi criado

Este template é adequado para:

- Livros acadêmicos ou técnicos  
- Livros-texto e material didático  
- Monografias e livros de pesquisa  
- Documentos extensos mantidos por várias versões  

É especialmente útil se você deseja:

- Uma estrutura clara e previsível  
- Escrita colaborativa via Overleaf  
- Builds reproduzíveis do documento  

---

## Estrutura do repositório

O projeto é organizado por responsabilidade, não por ordem de leitura.

```
.
├── main.tex
├── preamble.tex
├── bibliography.bib
│
├── frontmatter/
│   ├── title.tex
│   ├── copyright.tex
│   ├── dedication.tex
│   ├── epigraph.tex
│   ├── preface.tex
│   └── acknowledgments.tex
│
├── chapters/
│   ├── ch01-introducao.tex
│   └── ch02-capitulo.tex
│
├── backmatter/
│   ├── appendices.tex
│   ├── bibliography.tex
│   └── colophon.tex
│
└── figures/
```

---

## Como as partes se conectam

- **main.tex**  
  Arquivo raiz do projeto.  
  É o único arquivo que deve ser compilado e define a ordem das partes do livro.

- **preamble.tex**  
  Contém toda a configuração do documento: pacotes, layout, tipografia, cabeçalhos e metadados.  
  Nenhum conteúdo textual deve ser escrito aqui.

- **frontmatter/**  
  Contém os elementos pré-textuais, como capa, prefácio e agradecimentos.  
  A numeração de páginas usa algarismos romanos.

- **chapters/**  
  Contém o corpo principal do livro.  
  Cada capítulo deve estar em um arquivo separado.

- **backmatter/**  
  Reúne apêndices, referências e o colofão.  
  Capítulos nesta parte costumam ser não numerados ou identificados por letras.

- **bibliography.bib**  
  Base de dados BibTeX com as referências bibliográficas.

---

## Fluxo de escrita recomendado

1. Escreva conteúdo apenas nos arquivos dentro de `chapters/`, `frontmatter/` ou `backmatter/`
2. Não adicione pacotes ou comandos de layout fora de `preamble.tex`
3. Compile apenas o arquivo `main.tex`
4. Use rótulos e referências (`\label`, `\ref`) em vez de números fixos

Esse fluxo ajuda a manter o projeto organizado e escalável.

---

## Uso com Overleaf

Este repositório foi pensado para integração direta com o Overleaf.

Fluxo recomendado:

1. Crie um projeto no Overleaf
2. Clone o repositório e faça o upload dos arquivos no projeto
3. Use o Overleaf para edição e visualização

Evite editar o mesmo arquivo simultaneamente no Overleaf e localmente.

---

## Controle de versão

Este template pressupõe o uso de versionamento.

Boas práticas incluem:

- Mensagens de commit descritivas
- Tags para versões publicadas
- Registro de mudanças quando o livro for distribuído

O colofão pode ser usado para registrar informações de versão e build.

---

## Customização

Este template deve ser adaptado conforme o projeto.

Customizações comuns incluem:

- Alterar a classe do documento (`book`, `memoir`)
- Ajustar margens e tipografia
- Definir ambientes para teoremas, definições e exercícios
- Trocar o estilo de bibliografia
- Adaptar idioma e codificação

A estrutura em si é propositalmente genérica.

---

## Licença

Salvo indicação contrária, este template é fornecido como ponto de partida e pode ser reutilizado e adaptado livremente.

Ao utilizá-lo como base para um livro, recomenda-se definir uma licença apropriada para o conteúdo produzido.

---

## Observação final

Este template foi pensado para ser legível, previsível e durável. Uma estrutura que não precise ser repensada enquanto o livro está sendo escrito.

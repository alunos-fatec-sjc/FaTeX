# FaTeX
Modelo de TG da Fatec São José dos Campos - Prof. Jessen Vidal em Latex


### Exemplo do modelo genérico:
- [Fatec Trabalho Acadêmico](./example/fatec_trabalho_academico.pdf)

### Exemplo de TG utilizando esse modelo:
- [Segurança em Redes de IoT](https://www.dropbox.com/s/2zxeslq247yqsbi/FATEC%20-%20Seguran%C3%A7a%20IOT.zip?dl=0)

### Como editar?

Use alguns dos editores LaTeX:
- TexMaker
- Texstudio
- Atom (com plugins)
- Visual Studio Code (com plugins)

Ou um editor online:
- ShareLaTeX

### Agradecimentos:
- [Hideki Inoue](https://github.com/hiyoku)
- [Diogo Branquinho](https://github.com/diogobranquinho)
- Eduardo Sakaue
- [Giuliano Bertoti](http://giulianobertoti.github.io/)
- Emanuel Mineda
- [Filipe Meneses](https://github.com/filipemeneses)

### Comandos

#### `\tabela`

To render a table, it's required a title, caption, label and the contents, like so:

```latex
\tabela{<TABULAR>}{<TITLE>}{<CAPTION>}{tab:<LABEL>}
```

> Use `tabularx` for better rendering

##### Exemplo

```latex
\tabela{
  \begin{tabularx}{\textwidth}{|c|X|}
  \hline
  Exemplo de tabela com \texttt{tabularx} & O parâmetro X torna o texto justificado. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam faucibus a massa a iaculis. Praesent vel tempor metus, quis faucibus augue. Suspendisse eget tellus non metus volutpat ultrices. Vestibulum finibus laoreet maximus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec est purus, volutpat id sapien in, blandit mattis mi. Maecenas accumsan lobortis felis non pharetra. \\ \hline
  \end{tabularx}
}{Título da tabela}{Legenda da tabela}{tab:exemplo}
```

#### `\figura`

To render a figure, it's required a image path, caption, source and label, like so:

```latex
\figura{<IMAGE_PATH>}{<CAPTION>}{<SOURCE>}{tab:<LABEL>}
```

##### Exemplo

```latex
\figura{img/logo-fatec-sjc.jpg}{Exemplo de uso de figura}{Elaborada pelo autor}{fig:logo_fatec_sjc}
```

# Benvindu mai vizita MKDocs

## Atu Hahú ho MkDocs

MkDocs mak jeradór dokumentasaun nian ida ne'ebe foka ba simples no lalais liután. Iha karakterístika boot barak ne'ebé inklui:

- Preview dokumentasaun ita-nia ne'ebe ita hakerek ida-neʼe

- customiza Fasil ho tema no inefetivu 
- dokumentasaun ho Markdown

Notas

MkDocs mak opsaun ida ne'ebe boot atu hametin dokumentasaun ne'ebé tékniku. Maski nune'e, Lee Docs ne'e mós apoiu [Sphinx](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html), instrumentu ida seluk ba hakerek no harii dokumentasaun.

## Hahú informasaun lalais

Situasaun kona-ba imi iha ona Python, [instala MkDocs](https://www.mkdocs.org/#installation):

```
pip install mkdocs
```

Setup ita-nia projetu MkDocs:

```
mkdocs new .
```

This command creates `mkdocs.yml` which holds your MkDocs configuration, and `docs/index.md`which is the Markdown file that is the entry point for your documentation.

You can edit this `index.md` file to add more details about your project and then you can build your documentation:

Ukun-fuan ida ne'e kria `mkdocs.yml` ne'ebe mak ita-nia konfigurasaun MkDocs, no `docs/index.md` which ne'ebé mak hato'o Markdown ne'ebe mak pontu entrada ba ita-nia dokumentasaun. Ita bele edisaun ida-ne'e `index.md` husu atu fó hatene liután kona-ba ita-nia projetu no tuirmai ita bele harii imi-nia dokumentasaun:

```
mkdocs serve
```
Haruka harii imi-nia arkivu Markdown ba HTML no hahú server dezenvolvimentu ida ba browse ita-nia dokumentasaun. Loke  <http://127.0.0.1:8000/> iha ita-nia browser web atu haree imi-nia dokumentasaun. Ita bele halo mudansa ba ita-nia arkivu Markdown no ita-nia docs ne'ebe sei harii automatikamente fali.

![../_images/mkdocs-hello-world.png](https://docs.readthedocs.io/en/stable/_images/mkdocs-hello-world.png)

Ita-nia projetu MkDocs mak harii bainhira ita iha ita-nia dokumentasaun iha repository ida ne'ebe públiku hanesan GitHub, Bitbucket ka GitLab, ita bele hahú uza Read Docs nian husi [importasaun docs ita-nia](https://docs.readthedocs.io/en/stable/intro/import-guide.html).

## Rekursu esterna

- Iha neʼe iha rekursu esternál balu atu ajuda ita aprende tan kona-ba MkDocs.

-  [MkDocs dokumentasaun](https://www.mkdocs.org/) 

- [Markdown syntax matadalan](http://daringfireball.net/projects/markdown/syntax) 

- [Hakerek ba imi-nia docs ho MkDocs](https://www.mkdocs.org/user-guide/writing-your-docs/)

  

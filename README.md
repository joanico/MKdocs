# MKdocs

Hahú MkDocs

Mkdocs mak jerador situs static ida nebe dezeña ona hodi dezenvole situs web  dokumentasaun hanesan python no sira seluk. Iha língua programasaun python, MkDocs mak projetu open source ka rekursu ida ne'e nakloke ho apoiu barak hosi komunidade. Rekursu nebe uza hodi hakerek dokumentu sira mak uza rekursu markdown no konfigura uza rekursu yaml atu hatene konaba oinsa uza markdown bele lee nia referensia iha nee Markdown no  rekursu yaml bele hare iha ne'e Yaml.

Iha karakterístika boot barak nebe inklui:

- Bele host iha nebe deit
- Theme diak no disponibilidade hadia
- Dokumentasaun ho Markdown

Install Mkdocs

Install ho jerente pakote

Se karik uza ona pakote (hanesan  apt-get, dnf, homebrew, yum, chocolatey, no sira seluk) nee ita bele buka   install pakote refere konaba install "MkDocs" no bele hare nia versaun.

Se karik ita nia jestora pakote la iha pakote "MkDocs", ita bele uza nafatin ita boot nia pakote hodi instala "Python" no "pip". Depois ita bele uza pip hodi instala MkDocs. MkDocs suporta Python versions 3.5, 3.6, 3.7, 3.8, no pypy3.

Atu install mkdocs hanesan tuir mai no bele hare detallu husi instala MkDocs:

    $ pip install mkdocs

Hafoin install ita bele hare verzaun Mkdocs nebe ita foin install.

    $ mkdocs --version
    mkdocs, version 1.1.2 from /home/nicko/.pyenv/versions/Devel/envs/mkdocs/lib/python3.8/site-packages/mkdocs (Python 3.8)

Kria Projetu Foun

Kria projetu foun iha MkDocs hanesan tuir mai nee.

    $ mkdocs new Mkdocs
    $ cd Mkdocs

Konfigura mkdocs.yml ba ita nia projetu mkdocs mak hanesan docs/index.md ida nebe halo ho  Markdown parte pajina dahuluk ita nia dokumentasaun. 

    .
    └── MKdocs
        ├── docs
        │   ├── index.md
        └── mkdocs.xml

Ita bele edita file index.md no bele aumenta detallu konaba ita nia projetu no tuir mai ita bele hari ita nia dokumentasaun liu husi run mkdocs serve:

Exekuta Projetu

    $ mkdocs serve
    INFO    -  Building documentation...
    INFO    -  Cleaning site directory
    [I 160402 15:50:43 server:271] Serving on http://127.0.0.1:8000
    [I 160402 15:50:43 handlers:58] Start watching changes
    [I 160402 15:50:43 handlers:60] Start detecting changes

 Loke  http://127.0.0.1:8000/ iha ita nia browser web atu hare dokumentasaun. Ita bele halo mudansa ba ita nia file Markdown no ita nia docs nebe sei kria automatikamente. Bele hare rezultadu.



Aumenta dokumentasaun markdown foun

Mkdocs fo abilidade ba ita atu kontinua aumenta ita nia dokumentasaun ho rekursu markdown nian ba dokumentasaun nebe ita rai sei rai iha pasta ka directory docs

Bele hare exemplu :

    .
    └── MKdocs
        ├── docs
        │   ├── about.md
        │   ├── execute_python_syntax.md
        │   ├── index.md
        │   ├── python_advanced_tutorials.md
        │   ├── python_environment_setup.md
        │   ├── python_notifikasaun.md
        │   ├── python_other_tutorials.md
        │   ├── python_overview.md
        │   ├── python_tutorial.md
        │   └── python_variables.md
        └── mkdocs.yml

Kria nav ka menu

Iha exemplu leten ita aumenta ona dokumentasaun ho mardown iha directory docs nia laran hamutuk ho index.md tuir mai ita presiza defini hanesan menu ka dropdown menu iha mkdocs.yml nia laran hanesan iha exemplu tuir mai:

    site_name: Niko Docs
    # ida nee kria navbar ka menu
    nav:
    - Matadalan:
        - 'Python Tutorial': 'python_tutorial.md'
    - Python Baziku:
        - 'Python Introdusaun': 'python_overview.md'
        - 'Python Kria Enviromentu': 'python_environment_setup'
        - 'Python Sintase': 'execute_python_syntax.md'
        - 'Python Variabel': 'python_variables.md'
    - Python Avansadu:
        - 'Python Tutorial Avansadu': 'python_advanced_tutorials.md'
    - Python Tutorial Seluk:
         - 'Python Tutorial Seluk': 'python_other_tutorials.md'
    - Python Topiku:
        - 'Python Notifikasaun': 'python_notifikasaun.md'
    - Konaba:
        - 'Referensia': 'about.md'

Troka theme mkdocs

Ita bele troka theme iha mkdocs mak hanesan:

    #Kria tema 
    theme:
        name: readthedocs #iha nebe ita bele troka readthedocs tema ba mkdocs
        nav_style: red
        highlightjs: true
        hljs_languages:
            - yaml
            - rust

Kria extra css no Image

Iha mkdocs ita bele muda style tuir ita nia hakarak liu husi extra css ka ita bele uza image liu husi kria extra img iha mkdocs nia laran. Bele hare iha exemplu tuir mai ne'e.

    .
    └── MKdocs
        ├── css
        │   ├── theme.css
        │   └── theme_extra.css
        ├── docs
        │   ├── extra_css
        │   │   └── extra.css #Kria extra css 
        │   ├── img
        │   │   └── var.png   #Kria extra img
        │   ├── index.md
        │   ├── python_overview.md
        │   └── python_variables.md
        ├── fonts
        │   ├── fontawesome-webfont.eot
        ├── img
        │   ├── favicon.ico
        └── mkdocs.xyml

Exemplu troka style heading 2 husi markdown nia iha extra.css

    h2 {
    	color: red;
    }
    span.caption-text {
        color: cornflowerblue;
    }

Hari situs mkdocs

Hari ita nia dokumentasaun sai hanesan situs. Mkdocs sei fo aumatikamente dokumentu sira sei forma ho HTML index.html file no pasta ka directory no fo file static sira hanesan css, font, img ba directory.

Atu hari ita nia situs ita sei run mkdocs build no wainhira ita atu update ka aumenta dokumentasaun ruma ita presiza hamos directory tuan no koko hari fila fali maneira hamoos mak ita exekuta mkdocs buil --clean iha exemplu ida ne'e sei hatudu deit konaba oinsa hari ita nia situs.

    $ mkdocs build 

Sei hatudu rezultadu hanesan:

    $ ls
    404.html  css	fonts  index.html  mkdocs.yml  search.html  sitemap.xml
    about	  docs	img    js	   python      search		site

Deploy situs Mkdocs

MKdocs ita bele host Ita nia projetu bainhira ita nia dokumentasaun iha ona repository ida nebe públiku hanesan GitHub, Bitbucket ka GitLab, ita bele hahú uza Read Docs nian iha importasaun docs ita-nia ka deploy mkdocs

Iha dokumentasaun ida nee sei hatudu deit konaba deploy ba repository iha github nia mak hanesan kria repository foun kria github repository fo naran no tuir mai ita clone mai virtualenv local.

Nota: Atu deploy ho github ba dahuluk ita presiza kria file .gitignore atu nune la bele deploy hotu directory site/ ba ita nia repository. atu kria .gitignore mak hanesan:

    $ echo "site/" >> .gitignore

Atu deploy ita nia dokumentasaun ita exekuta

    $ mkdocs gh-deploy

Exekusaun kodigu ida leten iha kualker branch nebe deit maibe detallu iha master, ho mkdocs wainhira ita  deploy no run mkdocs gh-deploy sei kopia site ba branch gh-deploy no push ba github, gp-deploy nee autmatika wainhira ita run mkdocs gh-deploy. 

Hafoin ita deploy sei kria link ida refere ba ita nia account github nia exemplu https://joanico.github.io/MKdocs/  tuir mai ita bele ona asesu ita nia dokumentasaun iha kualker fatin ne'e deit.

Rekursu esterna

- Iha neʼe iha rekursu esternál balu atu ajuda ita aprende tan kona-ba MkDocs.
- MkDocs dokumentasaun 
- Markdown syntax matadalan 
- Hakerek ba imi-nia docs ho MkDocs



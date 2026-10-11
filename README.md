# Nom del projecte

El nom del projecte s’anomena Sobre Rodes.

# Eina utilitzada i versió

L’eina utilitzada és MkDocs i la seva versió és la 1.6.1.

# Comparativa breu amb els altres SSG

- **Hugo** és un generador de pàgines web estàtiques desenvolupat amb Go. Destaca principalment per la seva velocitat i flexibilitat, de manera que permet crear diferents tipus de webs, des de blocs fins a webs corporatives. Tot i això, al principi pot ser una mica més difícil d'aprendre a causa del seu sistema de plantilles.
- **Jekyll** és un generador desenvolupat amb Ruby que utilitza Markdown per crear pàgines web. És fàcil de començar a utilitzar i destaca per la seva integració amb GitHub Pages. També disposa de molts temes i connectors, però depèn de l'entorn Ruby i pot ser més lent quan es treballa amb webs grans.
- **MkDocs** és un generador desenvolupat amb Python que està orientat principalment a crear documentació tècnica. Utilitza Markdown i permet organitzar les pàgines mitjançant el fitxer `mkdocs.yml`. Un dels seus avantatges és que és senzill d'utilitzar i té una configuració clara. Tot i això, està més especialitzat en documentació que en altres tipus de webs.

En el següent enllaç es pot visualitzar la presentació dels SSG: https://canva.link/wmihsnvdh4lg5kw.

# Motiu de l’elecció de l’eina

En el nostre cas, hem escollit MkDocs per crear una pàgina web d'un concessionari de cotxes dedicat a la compra i venda de vehicles. Tot i que està més orientat a la documentació tècnica, ens permet organitzar el contingut en diferents pàgines i utilitzar Markdown per escriure la informació. Per tant, ens ha servit per crear una web estàtica senzilla i estructurada.

# Procés d’instal·lació

Per instal·lar MkDocs, només ha calgut executar la següent comanda a Git Bash:

```bash
pip install mkdocs
```

# Com executar la web localment

Per poder executar la web localment, només cal executar la següent comanda:

```bash
mkdocs serve
```

Aquesta comanda ens permet visualitzar els canvis realitzats a la web.

Per exemple, podem utilitzar una branca de proves que es pot anomenar QA per fer les modificacions sense que afectin la branca principal. Si tot ha funcionat correctament, només cal executar `git merge QA` dins de la branca `main`.

# Com generar la web

Per generar la web, només cal executar la següent comanda:

```bash
mkdocs gh-deploy
```

# Com publicar-la

Per publicar la web, només cal executar `mkdocs gh-deploy`. Després, cal situar-nos dins de la configuració del repositori i dirigir-nos a l'apartat Pages. A la secció Build and deployment, dins de Branch, només cal indicar que la branca és `gh-pages`.

# Com funciona el desplegament automàtic, si s’ha implementat

El projecte utilitza el workflow automàtic de GitHub Actions que s'anomena `pages-build-deployment`.

Quan s'executa la comanda `mkdocs gh-deploy`, MkDocs transforma els fitxers Markdown en pàgines HTML i els envia a la branca `gh-pages` juntament amb els recursos del tema. En aquell moment, GitHub Actions s'activa automàticament, processa el desplegament i publica la versió actualitzada de la web a GitHub Pages.

# Estructura del projecte

```text
web-estatica-Joan-Laia/
├── docs/
│   ├── img/
│   ├── index.md
│   ├── linux/
│   ├── xarxes/
│   ├── serveis/
│   └── blog/
├── mkdocs.yml
└── README.md
```

# URL de la web publicada

La web publicada es pot consultar en el següent enllaç: https://laiaknt.github.io/web-estatica-Joan-Laia/

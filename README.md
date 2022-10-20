# Japanese government datasets and news

For details see the [docs](#documentation).

## Data portals

- [e-Stat Portal Site](https://www.e-stat.go.jp/whats-new) ([RSS](https://www.e-stat.go.jp/news/rss/xml?refTarget=0101&haisinType=0100&category=all))
- [Tokyo Open Data Catalog](https://catalog.data.metro.tokyo.lg.jp/dataset) ([RSS](https://catalog.data.metro.tokyo.lg.jp/feeds/dataset.atom))

## Press Releases and News

- [Cabinet Office](https://www.cao.go.jp/index.html) ([RSS](https://www.cao.go.jp/rss/news.rdf))
- [Kantei](https://www.kantei.go.jp/) ([RSS](https://www.kantei.go.jp/index-jnews.rdf))
- [METI](https://www.meti.go.jp/press/index.html) ([RSS](https://www.meti.go.jp/ml_index_release_atom.xml))
- [Ministry of Finance](https://www.mof.go.jp) ([RSS](https://www.mof.go.jp/news.rss))
- [Ministry of Finance Policy Research Institute](https://www.mof.go.jp/pri/index.htm)

## Program Websites

- [Lonely deaths in Tokyo](https://www.fukushihoken.metro.tokyo.lg.jp/kansatsu/kodokushitoukei/index.html)
- [Furusato Nouzei Homepage](https://www.soumu.go.jp/main_sosiki/jichi_zeisei/czaisei/czaisei_seido/furusato/archive/)
- [National Police Stats](https://www.npa.go.jp/publications/statistics/sousa/statistics.html)
- [Local Adjustment Tax Homepage](https://www.soumu.go.jp/main_sosiki/c-zaisei/kouhu.html)
- [Tokyo Governor Expense Data](https://www.metro.tokyo.lg.jp/tosei/governor/governor/kosaihi/index.html)
- [Tankan Economic Survey](https://www.boj.or.jp/statistics/tk/index.htm/)

## Financial Timeseries

- [Bank Of Japan Timeseries](https://www.stat-search.boj.or.jp/index_en.html)

## Publications

- [METI Journal](https://journal.meti.go.jp/) ([RSS](https://meti-journal.jp/rss))
- [Nomura Research](https://www.nri.com/jp/knowledge/blog/lst?showall=True)
- [JRI Reports](https://www.jri.co.jp/report/year/) ([RSS](https://www.jri.co.jp/xml.jsp?id=12966))

## Report Aggregator

- [Keisai Report Watcher](http://www3.keizaireport.com/)

## Github accounts of Japanese government entities
From https://github.com/github/government.github.com/blob/gh-pages/_data/governments.yml#L340

- [city-of-kobe](https://github.com/city-of-kobe/)
- [codefornamie](https://github.com/codefornamie)
- [gsi-cyberjapan](https://github.com/gsi-cyberjapan)
- [nhohq](https://github.com/nhohq)
- [nims-dpfc](https://github.com/nims-dpfc)
- [wakayama-pref-org](https://github.com/wakayama-pref-org)


# Documentation

Resources are stored in `list.csv`. 

`readme/readme.py` generates this readme. 

`rss/opml.py` generates `list.opml`, which can be imported into a newsreader of your choice to follow resources with RSS feeds.

`changedetection/changedetection.py` loads the resources which do not have RSS feeds into the datastructure of a (changedetection.io)[https://github.com/dgtlmoon/changedetection.io]instance.

 `launch.sh` runs all the above and launches the [FreshRSS] newsreader (https://github.com/FreshRSS/FreshRSS) and the (changedetection.io)[https://github.com/dgtlmoon/changedetection.io] instance.

<!-- - TODO:
- 1-- Load rss feeds into fresh rss https://github.com/FreshRSS/FreshRSS/blob/edge/cli/README.md
- 2- Make a script that simultaneously launches change-detector and freshrss
- 3- Switch change-detector to docker version 
- 4- Launch change-detector and freshrss simultaneously with docker compose
- 5- Split the sites between those with an rss feed and those without. For those without, generate rss feed with change-detector. Then load all into freshrss. 
-->
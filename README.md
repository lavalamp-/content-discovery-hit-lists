content-discovery-hit-lists
=======================

This repository contains hit lists to use for web application content discovery.

## Common Crawl

Hit lists associated with mining [Common Crawl](http://commoncrawl.org/) data can be found in the `common-crawl` directory. Underneath the `common-crawl` directory, lists are separated out by which Common Crawl data set the list was generated from. These hit lists were generated using the [LavaHadoopCrawlAnalysis](https://github.com/lavalamp-/LavaHadoopCrawlAnalysis) and [lava-hadoop-processing](https://github.com/lavalamp-/lava-hadoop-processing) projects.

The syntax of the hit list file paths is as follows:

```
common-crawl/<common crawl data set>/<server type>/hit_list_<coverage percentage>
```

For instance, take the following file:

```
common-crawl/CC-MAIN-2014-49/apache_generic/hit_list_99.9
```

The contents of this file were generated from the `CC-MAIN-2014-49` Common Crawl data set and they comprise a hit list for Apache servers that do not specify an operating system. The URL paths found within the file are the most common URL paths (in descending order) associated with generic Apache servers as found in the `CC-MAIN-2014-49` crawl data. In total, the URL paths represent 99.9% of all observed URL paths.

More details will be available via a blog post on [lavalamp's personal blog](https://l.avala.mp/) in the near future.
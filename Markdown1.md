---
title: "My Markdown"
author: "Tim"
date: "12/14/2019"
output: 
  html_document: 
    keep_md: yes
---



## R Markdown

Now is the time.


```r
## insert your brilliant WORKING code here

require(tidyverse)
```

```
## Loading required package: tidyverse
```

```
## ── Attaching packages ────────────────────────────────────────────────────────── tidyverse 1.3.0 ──
```

```
## ✔ ggplot2 3.2.1     ✔ purrr   0.3.3
## ✔ tibble  2.1.3     ✔ dplyr   0.8.3
## ✔ tidyr   1.0.0     ✔ stringr 1.4.0
## ✔ readr   1.3.1     ✔ forcats 0.4.0
```

```
## ── Conflicts ───────────────────────────────────────────────────────────── tidyverse_conflicts() ──
## ✖ dplyr::filter() masks stats::filter()
## ✖ dplyr::lag()    masks stats::lag()
```

```r
# Create a small tibble.
# Here is another comment.
my_tibble <- tribble(
  ~x, ~y, ~z,
  "a", 2, 3.6,
  "b", 1, 8.5
)

my_avg <- my_tibble %>%
  summarize(ave_z = mean(z))

my_avg
```

```
## # A tibble: 1 x 1
##   ave_z
##   <dbl>
## 1  6.05
```


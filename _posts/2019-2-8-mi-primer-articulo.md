---
layout: post
title: Mi primer artículo
---

Este es mi primer artículo

## Sección 1

PROBANDO PROBANDO

### Subsección 1

``` r
resultados_segunda <- as_tibble(read.csv("ResultadosSegundaDivision.csv"))
resultados_segunda <- resultados_segunda %>% select(-X)

resultados_segunda$season <- as.character(resultados_segunda$season)
resultados_segunda$localTeam <- as.character(resultados_segunda$localTeam)
resultados_segunda$visitorTeam <- as.character(resultados_segunda$visitorTeam)
abis<-strptime(resultados_segunda$date,format="%Y-%m-%d")
resultados_segunda$date <- as.Date(abis,format="%Y-%m-%d")
```

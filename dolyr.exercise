install.packages("dplyr")
library(dplyr)
sessionInfo()

mtcars
mtcars %>% head()

dim(mtcars)
mtcars %>% nrow()
mtcars %>% ncol()
mtcars %>% names()
mtcars %>% class()


head(iris)
summary(head(iris))
mtcars %>% summary()
iris %>% summary()
iris %>% glimpse()

iris3 <- iris %>% filter(Sepal.Length > 2)
dim(iris3) 
history(100)

iris %>% group_by(Species) %>% summarize(MSL = mean(Sepal.Length))

iris %>% group_by(Species) %>% summarize(VarSL = var(Sepal.Length))

iris %>% group_by(Species) %>% summarize(SDSL = sd(Sepal.Length))

iris %>% group_by(Species) %>% summarize(MedSL = median(Sepal.Length))

iris %>% group_by(Species) %>% summarize(MedSL = median(Sepal.Length),
                                         VarSL = var(Sepal.Length),
                                         SDSL = sd(Sepal.Length),
                                         MSL = mean(Sepal.Length))


mtcars %>% group_by(cyl) %>% summarize(MMPG = mean(mpg),
                                       VarMP = var(mpg),                  
                                       SDMPG = sd(mpg),                 
                                       MedMPG = median(mpg)) 

mtcars %>% group_by(vs,am) %>% summarize(MedianMPG = median(mpg))

mtcars %>% select(1:4) %>% head(4)


mtcars %>% mutate( sqrtMPG= sqrt(mpg)) %>% head(4)

mtcars %>% mutate( sqrtQSEC= sqrt(qsec)) %>% head(5)

mtcars %>% mutate(sqrtMPG= sqrt(mpg), logMPG= log(mpg)) 
%>% select(mpg, sqrtMPG, logMPG, everything() ) %>% head(4)

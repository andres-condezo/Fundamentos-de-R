

mtcars <- read.csv("https://raw.githubusercontent.com/sap0408/mtcars/master/mtcars.csv", sep = ',')

rangeec <- read.table("https://raw.githubusercontent.com/sap0408/Orange-Economy/master/orangeec.csv", header =  TRUE, sep = ",")

# Una forma que encontré es con la librería dplyr donde hay un verbo que es Mutate, con el que puedes hacer conversión de variables y crear nuevas a partir de las actuales.
MtCars_Nuevo <- MtCars%>%
  mutate(vs = as.logical(am),
         am = as.logical(am))

# Cambiar de tipo de variable
rangeec$Country <- as.factor(orangeec$Country)

# ver la estructura de un dataset
str(nombreDelDataset)

# ver la clase de una variable
class(nombreDelDataset$nombreDeVariable)

# cambiar tipo de variable
nombreDataSet$variableActual = as.nuevaVariable(nombreDelDataSet$VariableActual)

# Summary de in data set
summary(nombreDelDataset)

# Cambiar de libras kilos 
mtcars$wt = (mtcars$wt*1000)/2 
mtcars.new <- transform(mtcars,wt=wt*1000/2)



# labdem.palette

`labdem.palette` es un paquete en R que proporciona la paleta de colores institucional del **Laboratorio de Métodos (LabdeM)** de la **FLACSO México**. Su objetivo es facilitar la generación de gráficos que respeten la identidad visual del laboratorio en contextos académicos, de comunicación y divulgación.

## 🚀 Instalación

Para instalar el paquete desde GitHub:

```r
# Instala devtools si no lo tienes
install.packages("devtools")

# Instala labdem.palette desde GitHub
devtools::install_github("LabdeM/labdem.palette")
```

library(labdem.palette)

# Ver la paleta completa
labdem_palette()

# Usar una paleta en ggplot2 (ejemplo básico)
library(ggplot2)

ggplot(mpg, aes(displ, hwy, color = class)) +
  geom_point(size = 3) +
  scale_color_manual(values = labdem_palette("categorical")) +
  theme_minimal()

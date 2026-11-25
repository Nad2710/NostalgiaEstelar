<img src="https://mmss.iimas.unam.mx/dmmss/wp-content/uploads/2026/02/cropped-LogoUNAM_IIMAS_Negro50-scaled-2.png" width="200"/>

### Fundamentos de Inteligencia Artificial
# Exposición: Sobre KNN, o la memoria obstinada y la nostalgia de la luz estelar
> Ramos González Nadia
>
> Profesores: Carlos Ricardo Cruz Mendoza y Noé Hernández Sánchez

---

*En memoria de esas estrellas brillantes que alguna vez estuvieron en el cielo o en la tierra, y que nos siguen contando historias del pasado.*

*En homenaje a todos los pies cansados que jamás dejarán de buscarlas.*

---

El presente repositorio reúne el material de la exposición final sobre el algoritmo **k-Nearest Neighbors (KNN)** para el curso de Fundamentos de Inteligencia Artificial. Inspirada en el documental *Nostalgia de la luz* de Patricio Guzmán, la exposición es una meditación sobre las posibilidades y las limitaciones del *machine learning*.

Incluye la presentación interactiva y el notebook con la implementación de KNN desde cero.

| Material | Descripción | Enlace |
|---|---|---|
| Presentación | Diapositivas interactivas de la exposición, en HTML | [`Presentacion/`](Presentacion/) |
| Notebook | Implementación de KNN desde cero sobre un cielo sintético de estrellas, galaxias y cuásares | [`RamosGonzalez_KNN_Estrellas.ipynb`](Notebook/RamosGonzalez_KNN_Estrellas.ipynb) |

## Sobre la exposición

La luz de las estrellas que vemos es un viaje al pasado: no nos muestra a la estrella como es hoy, sino como era cuando esa luz partió. Desde aquí, una estrella, una galaxia y un cuásar pueden verse igual, un pequeño punto de luz. KNN nos ayuda a reconocer qué es cada destello comparándolo con sus vecinos, y saber qué es cada uno es saber desde qué tan atrás en el tiempo nos está hablando.

En el desierto de Atacama se estudian dos pasados. Desde sus observatorios se estudia el pasado más pasado, el del universo, con herramientas como KNN. Y en esa misma tierra, las madres buscadoras reconstruyen el pasado menos pasado, el de nuestra sociedad, buscando fragmento por fragmento a sus desaparecidos. Las dos búsquedas miran al mismo cielo y pisan el mismo suelo; en Atacama se entrelazan.

Ahí también aparece el límite de nuestras herramientas. KNN sólo reconoce lo que alguien ya vio, midió y nombró: es un algoritmo de memoria obstinada. Hoy podemos clasificar estrellas a miles de millones de años luz, pero no ver lo que está bajo nuestros pies. Ojalá existiera un telescopio que nos ayudara a traspasar la tierra.

## Implementación

La presentación cubre la definición formal del algoritmo (métricas de Minkowski, selección de vecinos, regla de decisión, criterios de desempate, normalización, complejidad y teorema de Cover y Hart), un ejemplo paso a paso y aplicaciones en astronomía.

El notebook implementa KNN desde cero y lo prueba con 450 destellos sintéticos descritos por dos colores, $u-g$ y $g-r$:

| Métrica | Valor |
|---|---|
| Mejor k (validación) | 9 |
| Exactitud en prueba | 94.4 % |
| Coincidencia con scikit-learn | 100 % |
| Exactitud sin normalizar / normalizada | 34.4 % / 90 % |

```text
NOMBRE_DEL_REPO/
├── Presentacion/
│   ├── index.html                        # diapositivas de la exposición
│   └── img/                              # imágenes astronómicas
└── Notebook/
    └── RamosGonzalez_KNN_Estrellas.ipynb # implementación de KNN desde cero
```

## Referencias

- Guzmán, P. (2010). *Nostalgia de la luz* [Documental].
- Cover, T. y Hart, P. (1967). Nearest neighbor pattern classification. *IEEE Transactions on Information Theory*, 13(1), 21–27.
- Lourens, M. A. A. et al. (2024). Supervised star, galaxy, and QSO classification with sharpened dimensionality reduction. *Astronomy & Astrophysics*, 690, A224.
- Epps, B. S. (2016). La insoportable levedad de los huesos. *Cuadernos de Literatura*, 20(39).

Imágenes: NASA/SDO; NASA/JPL-Caltech; NASA, ESA, P. Oesch et al.; Y. Beletsky (LCO)/ESO.

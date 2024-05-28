# Importando la biblioteca de presentaciones
from pptx import Presentation
from pptx.util import Inches

# Crear una nueva presentación
prs = Presentation()

# Función para agregar una diapositiva con título y contenido
def agregar_diapositiva_titulo_contenido(titulo, contenido):
    diapositiva = prs.slides.add_slide(prs.slide_layouts[1])
    titulo_placeholder = diapositiva.shapes.title
    contenido_placeholder = diapositiva.placeholders[1]
    
    titulo_placeholder.text = titulo
    contenido_placeholder.text = contenido

# Diapositiva 1: Título
titulo = "La Reforma Protestante: Lutero, Calvino y el Anglicanismo"
diapositiva = prs.slides.add_slide(prs.slide_layouts[0])
diapositiva.shapes.title.text = titulo

# Diapositiva 2: Introducción a la Reforma Protestante
titulo = "Introducción a la Reforma Protestante"
contenido = (
    "- Contexto Histórico\n"
    "  - Siglo XVI en Europa\n"
    "  - Crisis de la Iglesia Católica\n"
    "  - Demandas de reforma interna\n"
    "- Causas Principales\n"
    "  - Corrupción en la Iglesia (venta de indulgencias)\n"
    "  - Desarrollo del humanismo renacentista\n"
    "  - Invención de la imprenta"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 3: Martín Lutero
titulo = "Martín Lutero"
contenido = (
    "- Biografía\n"
    "  - Nacimiento en 1483 en Eisleben, Alemania\n"
    "  - Monje agustino y teólogo\n"
    "- 95 Tesis (1517)\n"
    "  - Publicadas en Wittenberg\n"
    "  - Crítica a la venta de indulgencias\n"
    "  - Inicio de la Reforma\n"
    "- Principales Ideas\n"
    "  - Justificación por la fe\n"
    "  - Autoridad de las Escrituras sobre la Iglesia\n"
    "  - Sacerdocio de todos los creyentes"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 4: Impacto de Lutero
titulo = "Impacto de Lutero"
contenido = (
    "- Respuesta de la Iglesia Católica\n"
    "  - Excomunión (1521)\n"
    "  - Dieta de Worms\n"
    "- Consecuencias\n"
    "  - Traducción de la Biblia al alemán\n"
    "  - Formación de nuevas comunidades protestantes\n"
    "  - Inicio de guerras religiosas en Europa"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 5: Juan Calvino
titulo = "Juan Calvino"
contenido = (
    "- Biografía\n"
    "  - Nacimiento en 1509 en Noyon, Francia\n"
    "  - Abandono del catolicismo y mudanza a Ginebra\n"
    "- Obra Principal\n"
    "  - 'Institución de la Religión Cristiana' (1536)\n"
    "- Principales Ideas\n"
    "  - Predestinación\n"
    "  - Soberanía absoluta de Dios\n"
    "  - Disciplina eclesiástica y moral"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 6: El Calvinismo
titulo = "El Calvinismo"
contenido = (
    "- Difusión\n"
    "  - Europa (Suiza, Francia, Países Bajos, Escocia)\n"
    "  - Norteamérica (colonias puritanas)\n"
    "- Organización de la Iglesia\n"
    "  - Gobierno presbiteriano\n"
    "  - Énfasis en la educación y la ética del trabajo"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 7: El Anglicanismo
titulo = "El Anglicanismo"
contenido = (
    "- Orígenes\n"
    "  - Enrique VIII y el Acta de Supremacía (1534)\n"
    "  - Ruptura con el Papa por motivos políticos y personales\n"
    "- Desarrollo\n"
    "  - Reforma de la Iglesia de Inglaterra\n"
    "  - Fusión de elementos católicos y protestantes\n"
    "- Características\n"
    "  - Libro de Oración Común\n"
    "  - Doctrina de los Treinta y Nueve Artículos\n"
    "  - Estructura episcopal"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 8: Impacto del Anglicanismo
titulo = "Impacto del Anglicanismo"
contenido = (
    "- En Inglaterra\n"
    "  - Consolidación bajo Isabel I\n"
    "  - Tolerancia religiosa limitada\n"
    "- En el Mundo\n"
    "  - Expansión a través del Imperio Británico\n"
    "  - Influencia en la creación de la Comunión Anglicana"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 9: Comparación de Lutero, Calvino y el Anglicanismo
titulo = "Comparación de Lutero, Calvino y el Anglicanismo"
contenido = (
    "- Lutero\n"
    "  - Reforma interna de la Iglesia\n"
    "  - Enfocado en la fe y la escritura\n"
    "- Calvino\n"
    "  - Sistema teológico y disciplinario riguroso\n"
    "  - Predestinación\n"
    "- Anglicanismo\n"
    "  - Equilibrio entre tradición católica y reforma protestante\n"
    "  - Influencia política y cultural"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 10: Conclusión
titulo = "Conclusión"
contenido = (
    "- Legado de la Reforma\n"
    "  - Diversificación del cristianismo\n"
    "  - Influencia en la política, la cultura y la sociedad europea\n"
    "  - Desarrollo de nuevas corrientes y denominaciones protestantes"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Diapositiva 11: Preguntas y Discusión
titulo = "Preguntas y Discusión"
contenido = (
    "- Preguntas Abiertas\n"
    "  - ¿Cómo influyeron las ideas de Lutero en otras reformas?\n"
    "  - ¿Qué diferencias y similitudes ves entre el calvinismo y el luteranismo?\n"
    "  - ¿Qué impacto tuvo el anglicanismo fuera de Inglaterra?"
)
agregar_diapositiva_titulo_contenido(titulo, contenido)

# Guardar la presentación
prs.save('Reforma_Protestante_Lutero_Calvino_Anglicanismo.pptx')

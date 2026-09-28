# Editor memorial

Editor estático publicado en GitHub Pages. Guarda diseños y selección del PDF en localStorage por navegador.

## Plantilla del vaso medido

Diámetros exteriores de 6.2, 5.8, 5.1 y 4.3 cm a alturas acumuladas de 0, 3.5, 8.2 y 10 cm. El arco superior deseado mide 10 cm.

La opción «Mi vaso» desarrolla **tres troncos de cono independientes**, con 1.5 mm de separación de corte entre sus cajas. No es una pieza continua. Cada sector se calcula usando su altura inclinada `hypot(altura vertical, diferencia de radios)` y conserva la misma cobertura angular del vaso. Sus arcos superiores miden 10, 9.35484 y 8.22581 cm; el arco inferior final mide 6.93548 cm.

Recortar las tres piezas siguiendo el contorno, colocar sus centros alineados de arriba hacia abajo, sin superposición. Imprimir PDF a 100% / tamaño real con ancho 10 cm. El espacio de corte y la curvatura hacen que la caja exportada mida aproximadamente 11.4242 cm; no reducirla a un cuadrado de 10 cm. El exportador calcula esta escala automáticamente. Cambiar el ancho escala toda la plantilla, incluidas sus alturas.

Es una aproximación por tramos a partir de cuatro mediciones; no garantiza ausencia de arrugas sobre una superficie de curvatura continua. Probar en papel antes de usar adhesivo. Las miniaturas se reducen y no corresponden a la escala del vaso.

## Formas y exportación

- Vaso medido (3 secciones), cono ajustable, óvalo vertical, óvalo horizontal y rombo.
- Marcos generados específicos para óvalos y rombo; transparencia exterior.
- Selección independiente de 1 a 4 personas en el PDF, con imágenes principales o cinco miniaturas adicionales por persona.
- Paginación carta sin reducción automática. En óvalos se conserva la proporción; las miniaturas caben dentro de 4 × 4 cm.

Servir localmente: `python3 -m http.server 8873`.

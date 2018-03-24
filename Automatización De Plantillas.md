# Automatización Del Proceso De Diseño De Ofertas.

## Creación de la plantilla

Lo primero es crear la plantilla; es decir, el esqueleto común que compartirán todos los documentos individuales teniendo en cuenta que deberán variar algunos elementos: Imágenes, textos, números, etc.

## Precauciones al crear una plantilla

En Photoshop, una plantilla es un documento normal que se ha creado teniendo unas precauciones para que, cuando reciba los datos variables, no haya resultados inesperados y solo cambie lo que tiene que cambiar. Los principales requisitos y precauciones básicas son:

-   Cada elemento que recibirá un dato variable distinto debe estar aislado en una capa para él sólo. Cuando cambie el dato, cambiará el contenido de la capa al completo.
    
-   Los nombres que hacen referencia a un mismo elemento deben ser siempre iguales. El nombre que damos a cada capa debe ser exactamente el mismo que tenga la variable relacionada, en el campo de variable dentro de Photoshop y en la columna de variables del archivo de datos que las contienen y que importaremos. En esa denominación evitamos el uso de mayúsculas, espacios en blanco y caracteres con acentos o tildes como la ñ.
    
-   No debemos crear en el archivo de Photoshop variables que no se vayan a usar y tampoco podemos dejar variables sin usar en el archivo de datos —esto no es XML, que sí lo permite—; es decir: que si el archivo de datos contiene siete variables, hay que declarar siete variables válidas en el documento de Photoshop o eliminar del archivo de variables aquellas que no se vayan a usar en Photoshop. Dicho de otro modo: Tiene que haber una correspondencia de uno a uno.
    
-   Los textos variables van siempre en capas de texto. No se rasterizan nunca.
    
-   Los textos variables que deban o puedan ser un poco largos, se colocan dentro de cajas, nunca en trazados. Así, cuando las líneas sean demasiado largas, se partirán y continuarán en la línea siguiente. No se saldrán del documento. Por eso debemos prever un tamaño de caja razonable para el tamaño de los textos.
    
-   Es difícil que las variables de texto que vayan separadas en el documento de datos puedan formar una sóla variable en el documento de Photoshop; por ejemplo: Si queremos que el nombre y el apellido de las personas vayan juntas, deberán estar ya juntas en el documento de variables. No será posible unirlas en Photoshop.
    
-   Las modificaciones visuales de elementos variables como imágenes o textos procuramos hacerlas mediante efectos de capa. De ese modo es más fácil que cambie el contenido sin cambiar el aspecto.
    

## Los elementos de la plantilla de carnet para datos variables

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29472153_1601730243208894_8276500493056868352_n.jpg?oh=6ebbf7db6f23ab19afb9edeb043afe84&oe=5B37269C)

Una vez que se teiene la idea de la plantilla y de qué partes serán variables, creamos el documento en Photoshop conservando en capas separadas todos los elementos que creamos convenientes y, sobre todo, aquellos que vayan tratarse como variables, una por capa.


![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29388943_1601758309872754_6757702046037573632_n.png?oh=92c4000b5b448709bc49867c3332c02d&oe=5B289754)


Aquí se puede observar el esquema del documento que hemos creado. Hemos evitado el uso de acentos. 

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29468596_1601767209871864_7504034862341292032_n.jpg?oh=3074fd2a39bca83c5b886ad612ce632d&oe=5B3F1C07)

El grupo "`DISEÑO`" contiene los elementos básicos que no se modificaran estando de manera estatica. El grupo "`VARIABLES`" contiene todos los elementos que van a cambiar en la plantilla de cada producto de oferta.





## Preparación de los datos

### El archivo de datos

Los datos deben estar en formato de archivo de texto delimitado por tabulación. Cada línea forma un conjunto de registros que corresponden a un único producto. Las distintas variables o registro van separadas por tabulaciones. Este tipo de archivos suelen llevar la extensión  `*.txt`.


![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29468301_1601770506538201_4122814428271869952_o.jpg?_nc_cat=0&oh=75ead7e0d01272a87f3ff0deb8bae003&oe=5B3BE464)

Una hoja de cálculo como Microsoft Excel es una herramienta muy usual para la preparación de estos datos. Bastará con guardar la hoja de cálculo al formato "`Texto delimitado por tabulaciones`" para tener un archivo de datos que Photoshop sea capaz de importar.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29432902_1601774666537785_5109734983031848960_o.jpg?oh=e6fe723bf4f15fefdfe43f6e63a53c59&oe=5B36CCDC)

La primera línea se usa para identificar los registros por columnas: Articulo, Producto, PrecioUE, PrecioUD y Vigencia, No es necesario que aparezcan en el orden en el que se van a volcar en el documento de Photoshop, pero sí es imprescindible que se llamen igual y no sobre ni falte ninguno.


### Las imágenes

Volcar las imágenes a documentos con datos dinámicos sin prepararlas previamente es posible, pero no es recomendable. Mi consejo es estandarizarlas antes de volcarlas, igualándolas mediante un proceso por lotes con Photoshop. De este modo, sus dimensiones, modo de color y formato serán iguales y es más difícil que ocurran sorpresas.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29432923_1601776163204302_3932754458907246592_n.jpg?oh=707cee102a6ab5156dccb2f2f28a6511&oe=5B418BA7)

Las imágenes no van incluidas directamente en el archivo de datos. Lo que se incluye allí es una cadena de texto que hace referencia a su colocación en el ordenador, algo similar a “fotos/nombre\_de\_foto.jpg", ya que es buena idea colocar en una subcarpeta todas las fotografías, al mismo nivel que el archivo de datos. Eso facilita el control.

## La definición de variables en Photoshop

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29512251_1601785789870006_2933763568576757760_n.jpg?oh=fd26db40928e642843b5521891fe3bbd&oe=5B35834E)

Una vez terminado el documento de plantilla en Photoshop, vamos al menú “`Imagen – Variables`”. Lo primero que haremos es “`Definir`” las variables en la opción “`Capa`”.


Pulsamos y seleccionamos la capa que queremos definir como variable; por ejemplo: “`Producto`”. Como es un texto, seleccionamos la opción “`Sustitución de texto`” marcando esa casilla. Como nombre le damos exactamente el mismo nombre que la columna de datos que va a tomar, en ese caso “Producto”. Hacemos lo mismo con las demas capas.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29472094_1601784843203434_6733342911385042944_n.jpg?_nc_cat=0&oh=f9b7712ef61e86548e3996538f5eb6e0&oe=5B4779F2)

En el caso de la capa “articulo”, la opción que seleccionamos es “`Sustitución de píxel`” a la que Photoshop cambia automáticamente. La llamamos “`fotografía`” y elegimos la opción “`rellenar`” como se han recortado y preparado las imágenes previamene, no habra problemas.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t34.0-12/29134876_1605537859494799_1506252995_n.png?_nc_cat=0&oh=1735b0fc04360c7dc4f085c992716d71&oe=5AB888AD)

Cuando hayamos terminado, veremos que las capa variable asignada tienen un asterisco tras su nombre.

Pulsamos “`OK`” y guardamos el documento de Photoshop sin cerrarlo.

## La importación de los datos

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29389145_1601794976535754_2946095313036771328_n.jpg?_nc_cat=0&oh=305e497ed042af9a3cdcf40a46385edd&oe=5B48BF3E)

Volvemos al menú “`Imagen – Variables`” y seleccionamos la opción “`Conjunto de datos`”.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29496198_1601799669868618_5159315192143675392_n.jpg?_nc_cat=0&oh=2f4d9d398271444bc61f875103623a12&oe=5B3B5050)

Para traer los datos a la plantilla, pulsamos la opción “`Importar`”. En el siguiente cuadro de diálogo, buscamos el archivo en cuestión lo seleccionamos. Marcamos las casillas “`Usar la primera columna para nombres de conjuntos de datos`” y “`sustituir conjuntos de datos existentes`” esto último es para que no se nos empastelen los datos de otros conjuntos que hayamos podido estar trabajando antes. En codificación elegimos “`Automática`”.

### Posibles problemas

En la importación de datos variables a una plantilla es donde suelen surgir los problemas más simples y a la vez más difíciles de corregir.

Lo más usual es que se hayan creado variables de más o de menos, que los datos vengan separados por comas en vez de por tabulaciones o que la codificación del texto sea incomprensible para Photoshop.


### Comprobación de la importación

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29496461_1601802573201661_7232500900969840640_n.jpg?oh=cf99d74e7412e0ee920a97813350a998&oe=5B47EB36)

Hay dos maneras de hacer la comprobación de los datos. La más sencilla es nada más importar los datos, en esa mismo cuadro de diálogo. Vamos a la solapa “`Definir`” y allí mismo está la opción “`Conjunto de datos`”. Si pulsamos los triángulos al lado del “`Conjunto de datos`”, veremos que el nombre va cambiando, tomando el de la primera variable de cada conjunto de datos.

Si además hemos marcado la casilla "`Previsualización`", veremos como se producen los cambios en el mismo documento de Photoshop.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29425978_1601803963201522_8096171549490413568_n.jpg?oh=958ee5c36cdb66230921c38066f1dd17&oe=5B2E85C1)

La segunda manera es, una vez importados los datos, yendo al menú “`Imagen – Aplicar conjunto de datos`”. Pulsando sobre cada uno de los nombres, veremos como el aspecto del documento varía. Si todo es correcto, ya tenemos todo preparado.

## Creación de los documentos individuales

Photoshop sólo permite rematar el uso de los datos variables con plantillas mediante la creación de documentos individuales en formato nativo de Photoshop,  `*.psd`, uno por cada grupo de datos —“`conjunto de datos`”—.

![](https://scontent.fpbc2-1.fna.fbcdn.net/v/t1.0-9/29388875_1601806056534646_7681708244808499200_n.jpg?oh=61e5f7a2e7d7198bad1db0ef17daf8cb&oe=5B27AD10)

Vamos al menú “`Archivo – Exportar – Exportar conjuntos de datos como archivos`”. Allí veremos este cuadro de diálogo. Podemos elegir un único conjunto de datos o todos los conjuntos de datos. 

## Transformar los archivos en el formato deseado

El formato nativo de Photoshop es perfectamente válido para muchos trabajos, pero no siempre es el más compatible para enviar o para imprimir directamente. Por eso puede ser buena idea transformar las plantillas en otro como PDF. Los PDF de Photoshop modernos pueden mantener los datos vectoriales como tales, llevan las fuentes incrustadas y una excelente gestión del color, con lo que no se pierde nitidez o resolución.

La solución más sencilla es preparar una acción de Photoshop que permita guardar un archivo `*.psd`como PDF,a un estándar válido para imprenta que no obliga a ningún acoplamiento de transparencias ni a conversiones de color. Procesamos con ella todos los archivos en un proceso por lotes y tendremos las plantillas individuales.

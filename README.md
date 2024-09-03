# PROYECTO
#### El presente trabajo práctico tiene como objetivo aplicar los conceptos, principios y características del paradigma de la programación orientada a objetos (Clases, objetos, métodos, interfaz, herencia, polimorfismo, colecciones, etc.).

### Diagrama de clases UML:
https://drive.google.com/file/d/1bTTO6wg_ZR1USbBvrd_8WemuO4J9lQxR/view?usp=drive_link

## Objetivo
- Implementar todos los conceptos abordados del paradigma de la Programación orientada a objetos, como solución a un problema real, partiendo del análisis de la problemática, el diseño de la solución (Diagrama de clases) y posteriormente la construcción del producto final (Software).

## Procedimiento
### Investigación y Documentación
- Criptomonedas (criptodivisa o moneda virtual) es un término actual que refiere al dinero existente en un entorno digital. Actualmente posee un alto grado de utilización a causa de que se utiliza como medio de intercambio entre las empresas o instituciones. El valor de las criptomonedas es variable, el mismo se modifica en función de la demanda y la oferta de mercado, además del compromiso de los usuarios. 
- Las criptomonedas son el método de pago en una red descentralizada de ordenadores, conocida como blockchain o cadena de bloques, formada por nodos repartidos en todo el mundo.

### Algunos conceptos importantes:
- Nodos: Son ordenadores. Las personas que forman parte de los nodos, o los controlan, son conocidas como mineros.
- Exchanges: son empresas de cambio de divisas, permiten el cambio de dólares, euros u otras monedas fiduciarias por Cripto monedas. 
#### Algunas criptomonedas importantes
● BitCoin (BTS): Es la moneda pionera y por ende la de mayor valor. Es la moneda líder en el mercado de las criptodivisas.\
● Ethereum (ETH): No es una criptodivisa en sí, sino una plataforma de Blockchain (Cadena de cubo formada por ordenadores que funcionan como si fuera uno solo, y permite ejecutar aplicaciones dentro de esta red que se alimenta mediante el ether (su criptodivisa). Los tokens son activos digitales o unidades de valor, utilizados para realizar intercambios dentro de una cadena de Blockchain.\
● Dogecoin (DOGE): Es una moneda virtual que deriva del Litecoin, es famosa en redes sociales, alberga una gran comunidad. \
● Cardano (ADA): Es una plataforma de contratos inteligentes similar a Ethereum. Se enfoca en aumentar su seguridad a través de una arquitectura de capas (se autodenomina blockchain de 3° regeneración). La criptomoneda que utiliza es ADA.\
● Ripple (XRP): Es un método seguro que se destaca por su velocidad en las transacciones.\
● Tether (USDT): Fue creado como puente entre el dinero común y las criptomonedas, lo que provoca que estén respaldadas por una cantidad equivalente en dólares, euros o yenes. Por esto se conoce como la moneda estable o stablecoin.\
● Litecoin (LTC): Es la criptomoneda que posee la mayor liquidez y de la que es más simple de convertir a otras criptomonedas (a comparación de las otras). Resulta ser más veloz en los pagos.\
● Dash: Antiguamente conocida como xcoin o Darkcoin, supera a Bitcoin en la reducción de coste y tiempo de transacción. Posee una combinación de criptomonedas y procesos, que resulta casi imposible el rastreo de las transacciones, aumentando la privacidad del usuario.\
● Constellation (DAG): Es una cadena de bloques o blockchain descentralizada o distribuida e impulsada por un enfoque de microservicios.\
● Safemoon: Es un token de finanzas descentralizadas (DeFi). Esto significa que forma parte de un sistema financiero alternativo que permite el bloque de cadenas o blockchain sin la intervención de sistemas centralizados.

## Presentación
- Se solicita construir un sistema de administración y gestión de criptomonedas que le permita al usuario (Administrador o Trader) realizar transacciones de estas. La cantidad de criptomonedas presentes en el sistema es variable, inicialmente todas se encuentran confinadas en el archivo criptomonedas.csv Una posible representación del archivo podría ser:\
Bitcoin , BTC , 1245.00\
Ethereum , ETH , 1028.00\
Tether , USDt , 724.50
#### Cada criptomoneda se identifica por su nombre, símbolo, precio base en dólares a la fecha actual.
- En un segundo archivo mercados.csv se encuentra la información actual de cada criptomoneda en función de los parámetros del mercado (Capacidad, volumen en las 24 horas, Variación en los últimos 7 días). Un posible formato del archivo podría ser\
BTC , 1,38 , 34,66% , +13,84%\
ETH , 450,40 , 27,91% , +2,59% 
#### Dicho archivo contiene la misma cantidad de registros que el archivo criptomonedas.csv
#### Existen dos tipos de usuarios en el sistema: Un administrador que contiene como atributos un nombre y un perfil. El otro usuario es un trader que contiene como atributos el nombre, el número de cuenta bancaria, el nombre del Banco y el saldo actual (Considerar siempre positivo). Dichos usuarios se encuentran en el archivo usuarios.csv
Un posible formato podría ser:\
jperez, administrador\
hrizo24 , 7824621 ,Banco Río , 78000.00\
mlopez , 5821621, Banco Francés , 800000.00\
rlopez , administrador

#### En primera instancia el sistema debe solicitar el ingreso de los datos del usuario y determinar su perfil. En el caso de que el usuario sea administrador, el sistema exhibe un menú para la gestión de las criptomonedas (dar de alta, modificar, eliminar, consultar, ver mercado actual), y al usuario trader la posibilidad de consultar, ver mercado actual, recomendar, comprar y vender (también en formato de menú). En el caso de que el trader no se encuentre registrado en el sistema, deberá registrarse ingresando su nombre de usuario y los datos de su cuenta bancaria asociada: Número de cuenta, Nombre del banco y el saldo.
#### Un posible formato de menú para el administrador podría ser el siguiente:
#### Menú de opciones
-----------------------
1) Crear Criptomoneda 
2) Modificar Criptomoneda
3) Eliminar Criptomoneda
4) Consultar Criptomoneda
5) Consultar estado actual del mercado
6) Salir
Ingrese su opción (1 - 6): _

#### Las actualizaciones de los parámetros de las criptomonedas generan un impacto en el archivo mercados.csv del siguiente modo:
● Si el administrador desea agregar una criptomoneda en el archivo criptomonedas.csv, debe ingresar el nombre, el símbolo y el precio dólar base. La nueva criptomoneda se debe adicionar inmediatamente al archivo mercados.csv, en este caso los parámetros de capacidad, volumen en las 24 horas y variación en los últimos 7 días debe contener su valor base que es 1% en alza, la capacidad debe ser inicialmente 500. 
#### Nota: Si la criptomoneda que se desea dar de alta existe en el archivo criptomonedas.csv, se debe emitir un mensaje aclaratorio indicando que no se puede agregar y se debe consultar al usuario si desea modificar algún parámetro de esta, en caso afirmativo el sistema lo redireccionará a dicha funcionalidad.
● Si el administrador modifica algún parámetro de la criptomoneda (nombre, símbolo o precio dólar base), se deberá actualizar el símbolo de la criptomoneda en el archivo mercados.csv\
● Si el administrador elimina una criptomoneda del archivo criptomonedas.csv también se debe eliminar del archivo mercados.csv\
● Si el administrador o trader desea consultar los datos de una criptomoneda, el sistema debe confinar la información de los archivos criptomonedas.csv y mercados.csv\
Una posible representación de la consulta podría ser:\
Nombre: Bitcoin Símbolo: BTC Precio en dólares: 70.124,4\
Datos del mercado: Capacidad volumen en las últimas 24 horas Variación en los últimos 7 días 1,38 34,66% +13,84%
 
#### Por otra parte, el sistema ofrece al usuario trader realizar transacciones tales como comprar, vender, consultar y recomendar criptomonedas.
● Para la sección de compras, se debe seleccionar el símbolo de la criptomoneda y el total a comprar, el sistema debe exhibir el valor en dólares de esta y el total que se puede comprar (capacidad).\
○ En caso de que el usuario confirme la compra, la capacidad se debe restar en el archivo mercados.csv y aumentar un 5% los parámetros volúmen en las últimas 24 horas y variación en los últimos 7 días del mismo archivo. Si la cantidad de compras de una criptomoneda supera las 1000 entonces se debe aumentar su precio en dólares un 10%.\
○ El proceso para confirmar la compra es el siguiente: El sistema debe verificar que el usuario disponga de dinero en su cuenta bancaria, en caso contrario rechaza la operación y le solicitará al usuario ingresar el dinero faltante. Si la compra es satisfactoria, el sistema debe actualizar el saldo del usuario (disminuir el saldo) y almacenar todas las criptomonedas compradas hasta el momento por el usuario (a modo de archivo histórico) con el siguiente diseño:\
Símbolo de la criptomoneda y la cantidad comprada.
#### En el caso de que exista la criptomoneda en el archivo, solo se debe actualizar la cantidad (acumulando la anterior con la actual).
El nombre de dicho archivo debe ser NombreDeUsario_historico.csv\
Por último se debe actualizar el saldo del usuario en su cuenta bancaria.\
Un posible ejemplo del archivo histórico podría ser\
hrizo_historico.csv\
BTC , 35\
USDT , 5\
ETH , 23

● Para el caso de la venta, se debe seleccionar el símbolo de la criptomoneda y el sistema debe exhibir la cantidad máxima que puede vender. Dicha cantidad se debe obtener del archivo histórico del usuario. Luego, el usuario debe ingresar la cantidad a vender, si dicha cantidad es superior a la indicada se debe emitir un mensaje de error y continuar con la ejecución del menú. 
○ En el caso de que se confirme la venta, se debe aumentar la capacidad en el archivo de mercados.csv de dicha criptomoneda y disminuir un 7% el valor los parámetros volúmen en las últimas 24 horas y variación en los últimos 7 días. Luego de realizada la operación se debe actualizar el archivo histórico del usuario modificando la cantidad (disminuir la cantidad) y actualizar el saldo del usuario. 
● En el caso de que el usuario augure una recomendación de compra por parte del sistema, el mismo realizará una evaluación estadística entre la criptomoneda de mayor cotización y la cantidad disponible en el archivo de mercados.csv
#### El cálculo que se debe realizar es: (Cantidad disponible de la criptomoneda de mayor valor / precio en dólares de la criptomoneda) * 100
#### El sistema recomendará aquella criptodivisa de mayor porcentaje, tomando como referencia la del archivo criptomonedas.csv\
● El sistema le ofrecerá al usuario consultar/visualizar el archivo histórico de sus transacciones (Estado actual de las criptomonedas compradas y vendidas) ordenado alfabéticamente por símbolo o por cantidad en modo descendente.

#### Un posible formato de menú para el usuario trader podría ser el siguiente:
#### Menú de opciones
-----------------------
1) Comprar Criptomonedas
2) Vender Criptomonedas
3) Consultar Criptomoneda
4) Recomendar Criptomonedas
5) Consultar estado actual del mercado
6) Visualizar archivo de transacciones (histórico).
7) Salir
Ingrese su opción (1 - 7 ): _

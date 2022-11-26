# Tests jUnit con Cuenta Bancaria básica

El código fue realizado en Java 8 utilizando JUnit 5.

## Acerca de

La tarea consiste en construir un aplicativo del "Blue Bank" que permita realizar 2 tipos de transacciones electrónicas:

Retirar dinero desde cuenta
Depositar dinero en cuenta
Se debe tener en consideración que un usuario maneja dos tipos de cuentas (En 'CLP' y en 'USD').

## Test a implementar

|ítem	| Detalle| 
|---- | ---- |
|Test Inicialización|	|
|Test de Sesión	||
|Test Número de Operaciones por Sesión, en rango|	|
|Test Número de Operaciones por Sesión, valor límite||	
|Test Número de Sesiones, en rango	||
|Test Número de Sesiones, valor límite	||
|Test de Reinicio de Sesión	||
|Test depósito||	
|Test CantidadNoPermitida en CLP||	
|Test CantidadNoPermitida en USD||	
|Test CantidadNegativa en CLP	||
|Test CantidadNegativa en USD	||
|Test DespositoMontoCorrecto CLP||	
|Test DepositoMontoCorrecto USD||	
|Test DepositosIncrementos CLP|	Varias operaciones en test|
|Test DepositoIncrements USD|	Varias operaciones en test|
|Test DepositoMinimoPermitido CLP||	
|Test DepositoMinimoPermitidoUSD||	
|Test Retiro	||
|Test CantidadNoPermitida en CLP||	
|Test CantidadNoPermitida en USD	||
|Test CantidadNegativa en CLP	||
|Test CantidadNegativa en USD	||
|Test RetiroMontoCorrecto CLP	||
|Test RetiroMontoCorrecto USD	||
|Test RetiroDremento en CLP|	Varias operaciones en test|
|Test RetiroDremento USD|	Varias operaciones en test|
|Test RetiroMinimoPermitido CLP|	|
|Test RetiroMinimoPermitido USD	||
|Test RetiroMáximoPermitido CLP	||
|Test RetiroMáximoPermitido USD	||
|Test RetiroVaciadoDeCuenta USD	||
|Test RetiroVaciadoDeCuenta CLP	||
|Test Historico de Transacciones	||
|Test HistoricoTransaccionesInicio	||
|Test HistoricoTransaccionesDeposito  CLP||	
|Test HistoricoTransaccionesDeposito USD	||
|Test HistoricoTransaccioneRetiro CLP	||
|Test HistorioTransaccionesRetiro USD	||
|TestAplicativo|	|
|TestSet	|En caso de ser necesarios|
|TestGetters|	En caso de ser necesarios||

## Preparación
- Es necesario tener instalado [Gradle](https://gradle.org/)
- Clonar el repositorio en la carpeta deseada, desde la consola:
```
git clone https://github.com/rettke/TestJUnitExample
```
- Acceder a la carpeta del proyecto:
```
cd ./TestJUnitExample
```

## Ejecución
Para correr, ya en la carpeta desde la consola ejecutar:
```
gradle run --console=plain
``` 
Para así iniciar la ejecución del programa por consola.

## Pruebas
Para ejecutar las pruebas se debe utilizar el comando:
```
gradle test
```
Al ejecutar las pruebas se genera el archivo:
```
./build/reports/tests/test/index.html
```
Este archivo contiene un reporte con los resultados de todas las pruebas ejecutadas, simplemente abrirlo con cualquier navegador web.

## Archivos proyecto
Se trabajó principalmente en tres archivos,  en ``./src/main/java/test/cuenta/bancaria/`` se encuentra:
- `Cuenta.java`, el cual contiene la lógica del manejo de la cuenta bancaria.
- `Main.java`, el cual utiliza la clase Cuenta y controla la interacción con el usuario.

Por otro lado, en `./src/test/java/test/cuenta/bancaria/`:
- `CuentaTest.java`, que contiene todas las pruebas unitarias.

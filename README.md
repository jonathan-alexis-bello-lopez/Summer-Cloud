# SUMMER CLOUD APUNTES


![img-banner](README.assets/image-20210709233811955.png)

## Summer Cloud Cracks TEAM!
![THE TEAM](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTt4C49JK8nTSi6M14D9gbctGUXpa4KWiHioA&usqp=CAU)

## Integrantes
- Sergio Manuel López
- Ilai Alanis
- José Armando Díaz
- Paola Salas
- Jonathan Alexis Bello López

## Introducción a Azure

### ¿Qué es Azure?
Es una plataforma de informática en la nube con un conjunto de servicios que sirve para ayudarle a crear soluciones que satisfagan los objetivos empresariales.
Azure proporciona una gran cantidad de servicios basados en la nube, como el almacenamiento remoto, el hospedaje de bases de datos y la administración centralizada de cuentas.

![Microsoft Azure](https://www.wwt.com/api/attachments/60d22db389a4c300876888b9/file)

## ¿Qué es la informática en la nube?

Es la entrega de servicios informáticos a través de Internet, lo que se conoce como la nube. Estos servicios incluyen servidores, almacenamiento, bases de datos, redes, software, análisis e inteligencia. La informática en la nube ofrece una innovación más rápida, recursos flexibles y economías de escala.
Beneficios de usar la informática en la nube:

- Reducir los costos operativos.
- Ejecutar la infraestructura de forma más eficaz.
- Escalar a medida que cambien las necesidades empresariales.

Dicho de otro modo, la informática en la nube es una forma de alquilar potencia de proceso y almacenamiento de un centro de datos de terceros. Los recursos de la nube se pueden tratar igual que los recursos de un centro de datos propio. Cuando haya terminado con ellos, solo hay que devolverlos. Únicamente se le cobrará por lo que use.

## ¿Qué puedo hacer con Azure?

Azure proporciona más de cien servicios que permiten hacer todo tipo de cosas: desde ejecutar las aplicaciones existentes en máquinas virtuales hasta explorar nuevos paradigmas de software, como bots inteligentes y realidad mixta.

## ¿Qué es Azure Portal?

Azure Portal es una consola unificada basada en web que proporciona una alternativa a las herramientas de línea de comandos. Con Azure Portal, puede administrar la suscripción de Azure mediante una interfaz gráfica de usuario. Puede:

- Compile, administre y supervise todo, desde aplicaciones web sencillas hasta complejas implementaciones en la nube.
- Cree paneles personalizados para una vista organizada de recursos.
- Configure opciones de accesibilidad para una experiencia óptima.

Azure Portal está diseñado para proporcionar resistencia y disponibilidad continua. Mantiene una presencia en todos los centros de datos de Azure.

## Componentes de la arquitectura de Azure

Antes de comenzar a describir la arquitectura, vamos a describir los siguientes conceptos para poder comprender mejor este tema:
- Recursos: Son los recursos son instancias de servicios creados, como máquinas virtuales, almacenamiento o bases de datos SQL.
- Grupos de recursos: Los recursos se combinan en grupos de recursos, que actúan como un contenedor lógico en el que se implementan y administran recursos de Azure.
- Suscripciones: Estas se refieres a las cuentas de usuario y los recursos que han sido creados por los usuarios. Para cada suscripción, existen límites y/o cuotas en la cantidad de recursos que se lleguen a usar. Una cuenta puede tener una suscripción o varias suscripciones que tienen diferentes modelos de facturación y a las que se aplican diferentes políticas de administración de acceso. Puede usar las suscripciones de Azure para definir límites en torno a los productos, servicios y recursos de Azure.
- Grupos de administración: Ayudan a administrar el acceso, la política y el cumplimiento de las suscripciones. 
<br>

Dicho esto, podemos continuar con la descripción de los componentes, los cuales son:
 - **Regiones de Azure**
 <p> Las regiones de Azure son un conjunto de centros de datos implementados dentro de un perímetro definido por latencia, y se conectan a través de una red de baja latencia. Actualmente hay 42 regiones disponibles en todo el mundo.</p>
  
 - **Regiones de emparejamiento**
 <p>Como ya sabemos Microsoft opera centros de datos todo el mundo, esto incluye a Azure que cuenta con muchas ubicaciones diferentes. Una ubicación en Azure se refiere a un área donde se encuentra al menos una región de Azure. Una región de Azure se refiere a un área dentro de una geografía que contiene uno o más centros de datos de Azure.
<br>
Para facilitar la alta disponibilidad, cada región de Azure se empareja con otra región que se encuentra cerca. Este emparejamiento se denomina "regional pair".<br>
Los "regional pair" permiten que Azure serialice las actualizaciones de la plataforma y el mantenimiento planificado. </p>

 - **Regiones disponibles**
 <p> Availability Zones es una oferta de Azure que se utiliza para proteger las aplicaciones y los centros de datos de las fallas del centro de datos. Cada zona de disponibilidad es una ubicación física única dentro de una región de Azure, y cada zona es compatible con uno o más centros de datos.<br>
Las zonas de disponibilidad son centros de datos físicamente separados dentro de una región de Azure. Cada zona de disponibilidad se compone de uno o más centros de datos equipados con alimentación, refrigeración y redes independientes. Si una zona se cae, la otra sigue funcionando. <br>
Cada zona de disponibilidad dentro de una región de Azure se compone de una combinación de dominios de error y dominios de actualización.<br>
Se pueden utilizar las zonas de disponibilidad para ejecutar aplicaciones con un trabajo crítico y crear alta disponibilidad en la arquitectura de su aplicación colocando sus recursos informáticos, de almacenamiento, de red y de datos dentro de una zona y replicando en otras zonas. <br>
Las zonas de disponibilidad son principalmente para máquinas virtuales, discos administrados, balanceadores de carga y bases de datos SQL. Los servicios de Azure que admiten zonas de disponibilidad se dividen en dos categorías: Servicios de zona y Servicios con redundancia de zona. 
</p>
 
 - **Grupo de recursos**
 <p> Los grupos de recursos son contenedores lógicos en Azure. Contienen recursos de Azure relacionados que forman parte de una solución de Azure más grande. Estos grupos de recursos pueden hospedar todos los recursos que componen una solución de Azure, o también pueden hospedar solo los recursos que deben administrarse como parte de un grupo.
<br>
Al trabajar con grupos de recursos de Azure, hay algunas cosas a considerar, como por ejemplo, dado que todos los recursos dentro de un solo grupo de recursos generalmente comparten un ciclo de vida similar, es importante determinar el ciclo de vida de los recursos que planea colocar en un solo grupo de recursos. </p>
 
 - **Administrador de recursos**
  <p> Dentro de Azure, existen varios componentes que proporcionan la infraestructura para una aplicación o servicio que se ha implementado en Azure. 
Debido a que todas estas partes funcionan juntas para brindar una solución, generalmente se implementan, administran y monitorean todos estos recursos como un grupo. El administrador de recursos es una herramienta que le permite trabajar con todos los recursos subyacentes que forman parte de una solución como grupo. Con el administrador de recursos, puede implementar, actualizar e incluso eliminar todos los recursos que forman una solución en una sola operación coordinada.</p>


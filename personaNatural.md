

## Estándar para el Registro de la Persona Natural

Los estándares listados en este documento han sido consensuados por representantes de MINEC, INJUVE, ISDEMU, ISNA, MOP, MH, MTPS, MINED, SETEPLAN entre otras desde la comisión  para la estandarización de procesos del Comité Intersectorial del Subsistema de Protección Social.  Asi mismo se ha ratificado, compartido, mejorado y consensuado en la mesa de líderes de Datos Abiertos en la que participan líderes de tecnología de instituciones como Ministerio de Hacienda, Comisión Portuaria Autónoma, Instituto Salvadoreño del Seguro Social, Ministerio de Obras Publicas y Ministerio de Salud. 

Puede agregar sus consultas en esta plataforma o directamente a la Dirección de Gobierno Electrónico, 2511 5073.  


###  1. Nombre 

Estructura:
1. Primer nombre 
2. Segundo Nombre 
3. Tercer Nombre 
4. Primer Apellido 
5. Segundo Apellido 
6. Apellido de Casada 
7. Persona Responsable (si aplica)
8. Conocido por según DUI (si aplica)

Norma: No aplica  
Tipo de dato: Alfanumerico  
Ejemplo: Mario Perez  

*Cada nombre o apellido deberá ser almacenado en un campo individual*

###  2. Fecha de Nacimiento   
Estructura: «YYYY-MM-DD»  
Norma: ISO 8601  
Tipo de dato: Alfanumerico  
Ejemplo: 2018-05-07  

*Donde YYYY representa el año, MM el mes y DD el día del mes*
    
###  3. registro de Identificador para paises   
Tipo: ALFA   
Estructura: XX   
Norma: ISO 3166-1 "códigos alfa-2", tanto los vigentes como los reservados   
Ejemplo de uso: SV   
Tamaño nimino: 2   
Tamaño maximo: 2   

###  4.  Registro del Sexo de una persona   
Tipo: Alfanumerico   
Nombre: Sexo   
Definición: De acuerdo con la Organización Mundial de la Salud (OMS) el término “sexo” se refiere al "conjunto de características biológicas que definen al espectro de humanos como hembras y machos".  Sexo con el que nació una persona para fines administrativos o legales.   
Estructura:    
Codigo 1, 2, 0, 9      
1 para Masculino    
2 para Femenino      
0 para Desconocido   
9 para sexo no aplicable   
Norma: ISO 5218   
Comentario: Sexo de una persona como consta en su DUI para nacionales, Partida de nacimiento para menores o CUN, pasaporte para extranjeros o carne de residente.   

###  5. Registro del Genero de una persona   
Tipo: Alfanumerico   
Nombre: Genero   
Definicion: Orientación que tiene la persona sobre sí mismo que podría no coincidir con sus características sexuales o con su Sexo
Estructura:   
Codigo 1, 2   
1 para genero masculino   
2 para genero femenino   
Norma internacional: N/A   
ejemplo de uso: 2 Femenino   
Comentario: El género lo debe de expresar por voluntad propia la persona y no debe de quedar a discreción de ningún otro. Una persona en cuyo caso puede ser Sexo masculino y género femenino.    

###   6.  Código de Identificación de la persona   
Para menores de edad:      
  Nombre de uso: Codigo Unico del Nacimiento    
  Abreviatura: CUN   
  Tipo: Numerica   
  Estructura: DDMMAAAACCCV   
  Norma: Acuerdo de creación CUN Ministerio de Salud    
  Ejemplo de Uso: 01012017001X   
  Tamaño minimo: 12   
  Tamaño maximo: 12   
  Comentario: Obligatorio para menores de edad, asignado por MINSAL   

Para mayores de edad Salvadoreños   
  Nombre de uso: Documento Unico de Identidad   
  Abreviatura: DUI   
  Tipo: Numerica   
  Estructura: #########   
  Norma: Ley de Esp. Reguladora de la emisión del DUI    
  Ejemplo de Uso: 002883129  (el ultimo digito como verificador)   
  Tamaño minimo: N/A   
  Tamaño maximo: N/A   
  Comentario: Obligatorio para mayores de edad, asignado por RNPN   

  Nombre de uso: Numero de Identificación Tributaria    
  Abreviatura: NIT   
  Tipo: Numerica   
  Estructura: ####-######-###-#   
  Norma: Ley de creación del NIT   
  Ejemplo de Uso: 0614-040282-105-0   
  Tamaño minimo: N/A   
  Tamaño maximo: N/A   
  Comentario: Obligatorio para mayores de edad, asignado por Ministerio de Hacienda   
  
Para extrageros no perteniecientes al CA4   
  Nombre de uso: Pasaporte   
  Abreviatura: N/A   
  Tipo: Alfanumerico   
  Estructura: x############   
  Norma: OACI   
  Ejemplo de Uso: A002883129   
  Tamaño minimo: N/A   
  Tamaño maximo: N/A   
  Comentario: Obligatorio para extrangeros que no pertenezcan al bloque CA4 Guatemala, Honduras, Nicaragua, El Salvador   
    
Para extrangeros pertenecientes al bloque CA4 Guatemala, Honduras, Nicaragua    
  Nombre de uso: Cedula   
  Abreviatura: N/A   
  Tipo: Alfanumerico   
  Estructura: x############   
  Norma: Acuerdo Regional CA4   
  Tamaño minimo: N/A   
  Tamaño maximo: N/A   
  Comentario: Obligatorio para extrangeros que pertenezcan al bloque CA4 Guatemala, Honduras, Nicaragua, El Salvador   
 
 Para personas nacionales, exterangeras, menores y mayores de edad que reciben beneficios sociales por parte del Gobierno Salvadoreño   
  Nombre de uso: Código de Registro Único de Participantes   
  Abreviatura: RUP       
  Tipo: Numérica   
  Estructura: ########   
  Norma Internacional: Lineamientos de Gobierno para el Registro Unico de participantes    
  Comentario: Codigo asignado por la Secretaria Tecnica y de Planificación de la Presidencia   
  
###  7. Registro del Estado Familiar de la persona        
Tipo: Alfanumerico   
Estructura:   
Codigo 1, 2, 3, 4, 5, 6 donde   
1 para Acompañada(o)   
2 para Casado(a)   
3 para Viuda(o)   
4 para Divorciado(a)   
5 para Separada(o)   
6 para Soltera(o)   
Norma: Codigo de Familia y Ley Procesal de Familia   
Tamaño minimo: 8 caracteres   
Tamaño maximo: 13 caracteres   

###  8. Registro domiciliar   
Tipo: Alfanumerico   
Estructura:   
Departamento: ##   
Municipio: ####(dos dep. + dos de municipio)   
Canton: ###### (2 dep. + 2 muni. + 2 cantón)   
Cacerío: XX# - ######## - ########_## (los últimos dos es Asentamiento Urbano Precario)        
AUP: #### (los últimos dos dígitos es departamento)      
Dirección: XXX  (dirección actual de residencia)   
NIC/NIS del recibo de electricidad: ###########        
Nombre de la compañia electrica:      
Norma: Catálogo de DIGESTYC, Mapa de Pobreza Urbana y Exclusión Social 2012   
Comentario: AUP: Asentamiento urbano Precario, de Acuerdo al mapa de pobreza Urbana y Exclusión Social 2012.   
Departamento, dirección y municipiop de carácter obligatorio.   
Canton, cacerio, AUP, NIC/NIS de carácter obligatorio para los registros o controles de beneficios sociales.    
Departamentos, municipios y cantones se utilizará la lista oficial de cantones de la DIGESTYC  acuerdo del 2007.   

###   9. Registro de contacto   
Estructura:
Correo Electrónico: xx@xx.xxx    
Tipo Alfanumerica   
Teléfono fijo: ########   
Teléfono movil: ########   
Tipo Numerica       
Compañia telefonica: xxxxxxxxxx       
Tipo Alfanumerica 
Norma internacional: ITU E.164 (teléfono) RFC 5322 (correo)    
Ejemplo de uso: nelsonperez23@gmail.com
Tamaño minimo: N/A   
Tamaño maximo: N/A   
Comentario: Las instituciones deberán prever e invertir en el envió de mensajes como recordatorios vía SMS a sus usuarios   

###   10.  Registro del nivel educativo de una persona   
Tipo: Alfanumerico   
Estructura:   
Codigos 0, 1, 2, 3, 4, 5, 6, 7, 8, 9  donde  
0 para Educación Inicial   
1 para Parvularia (1° A 3°)   
2 para Básica (1° a  9°)   
3 para Media (10° a 13°)   
4 para Superior Universitaria (1° a 9° año universitario) (10° a 12° Maestría) (13° a 15° Doctorado)   
5 para Superior No Universitario (1° a 3°)   
6 para Educación Especial (ciclo I, II, III y IV)   
7 Ninguno   
8 otros   
9 Curso de nivelación   
Norma internacional: N/A   
Comentario: La institucion referente del estandar para esta escala es el MINED   

###   11.  Estado del registro la persona    
Estado del registro: 1, 2   
1 para Activo   
2 para Inactivo     
  
## Licencia

Este trabajo esta cubierto dentro de la estrategia de desarrollo de servicios de Gobierno Electrónico del Gobierno de El Salvador y como tal es una obra de valor público sujeto a los lineamientos de la Política de Datos Abiertos y la licencia [CC-BY-SA](https://creativecommons.org/licenses/by-sa/3.0/deed.es).  

# ISRH-Dipas
Base de datos de estaciones meterolÃ³gicas de la Provincia de CÃ³rdoba

Database: **hidricos**

Tabla: _**hv_continetes**_ (5) Continentes
- _continente_: abreviación (AF, AM, etc)
- _nombre_: completo (Africa, América, etc)

Tabla: _**hv_cuenca**_ (24) Cuencas
- _id_: identificación
- _cuenca_: nombre de la cuenca

Tabla: _**hv_dptospartidos**_ (3657) Departamentos
- _dpto_partido_: id partido???
- _nombre_: nombre del partido/departamento
- _provincia_: provincia ID
- _estado_: letra identificatoria ???
- _nombre_: nombre de la cuenca

Tabla: _**hv_estacion**_ (908) Estaciones
- _id_estación_: id de la estación
- _codigo_: código de estación, que difernecia con id??
- _n_dpto_: link a dpto_partido?
- _dpto_: nombre del departamento, repetido?
- _n_cuenca_: link a id cuenca?
- _cuenca_: Nombre de la cuenca
- _nombre_: nombre de la estación
- _long_deg_: longitud, precisión (esta al reveee!!)
- _lat_deg_: latitud, precisión (esta al reveee!!)
- _lon_: redondeado, (crearon campos nuevos :S)
- _lat_: redondeado, (crearon campos nuevos :S)
- _msnm_: altitud
- _institución_: a quien pertenece
- _red_: red a la que pertenece (red_id?)
- _campaa_: número ???
- _num_maq_: número de???
- _id_ant_: número de???

Tabla: _**hv_estacion_correlacion**_ (3665) ???????
- _id_: fila id
- _codigo_: codigo fila
- _id_anterior_: num ident??
- _id_actual_: num ident??
- _repetido_: nsnc??
- _codigo_actual_: nsnc??
- _num_maq_: nsnc??
	
Tabla: _**hv_estacion_origen**_ (753) Localidades? casi igual a estacion
- _id_: fila id
- _id_estación_: id de la estación
- _codigo_: código de estación, que difernecia con id??
- _n_dpto_: link a dpto_partido?
- _dpto_: nombre del departamento, repetido?
- _n_cuenca_: link a id cuenca?
- _cuenca_: Nombre de la cuenca
- _nombre_: nombre de la estación
- _long_deg_: longitud, precisión (esta al reveee!!)
- _lat_deg_: latitud, precisión (esta al reveee!!)
- _lon_: redondeado, (crearon campos nuevos :S)
- _lat_: redondeado, (crearon campos nuevos :S)
- _msnm_: altitud
- _institución_: a quien pertenece
- _red_: red a la que pertenece (red_id?)
- _campaa_: número ???
- _num_maq_: número de???
- _id_ant_: número de???

Tabla: _**hv_groups**_ (empty)

Tabla: _**hv_groupsmembers**_ (empty)

Tabla: _**hv_localidades**_
 - _localidad_ : localidad id
 - _nombre_ : nombre
 - _nombre_abreviado_ : nombre abreviado 	
 - _dpto_partido_ : id
 - _ddn_ : ???

Tabla: _**hv_log**_ (32) registros de???
- _id_: id 
- _time_: timestamp
- _userid_: id de usuario
- _ip_: ip 
- _module_: modulo
- _action_: acción
- _url_: dirección
- info: ??

Tabla: _**hv_logdisplay**_ (94) resigtros de?
- _module_: modulo
- _field_: campo
- _action_: acción 
- _mtable_: mtable

Tabla: _**hv_hvmediciones**_ (126067)
- _id_: fila id
- _id_estación_: link id estacion
- _id_variable_: link id variable
- _id_usuario_: link id usuario
- _anio_: año de la medición
- _mes_: mes de la medición
- _fecha_registro_: día de la carga del dato (día/mes/año)
- _hora_registro_: (empty)
- _dia1_ : día de la medición
- _.._
- _dia31_
- _num_maq_: id ???
- _id_ant_: NULL

Tabla: _**hv_mediciones_log_error**_ (392)
IDEM ANTERIOR

Tabla: _**hv_mediciones_origen**_ (1)
IDEM ANTERIOR

Tabla: _**hv_modules**_
- _id_: id
- _name_:  nombre del módulo
- _version_: 
- _cron_
- _lastcron_
- _search_
- _visible_

Tabla: _**hv_paises**_ (184)
- _nombre_: nombre del país
- _continente_: id continente en el que s eencuentra
- _codigo_iso_: codigo

Tabla: _**hv_persona**_ (2)
- _id_
- _nombre_
- _apellido_
- _dni_

Tabla: _**hv_precipitacion**_ (2537261)
- _id_
- _id_usuario_
- _id_estacion_
- _fecha_registro_: fecha en que se cargo
- _hora_registro_: todo en 1899??
- _mes_: mes medición
- _anio_: año medición
- _lluvia_: 1/0??
- _nieve_: 1/0??
- _granizo_: 1/0??
- _llovizna_: 1/0??
- _neblina_: 1/0??
- _tormenta_: 1/0??
- _helada_: 1/0??
- _nro_dia_: día del mes?
- _hora_: hora ?
- _hora_ini_: hora inicio
- _min_ini_: min inicio
- _hora_fin_: hora fin
- _min_fin_: min fin
- _durac_hora_: diff
- _durac_min_: diff
- _cant_mm_: medición en mm
- _altura_: altura de??
- _acumulada_: 
- _observ_: ??
- _operador_: quien hizo la mediciómn
- _num_maq_: id maquina?? que es??
- _id_ant_: NULL

Tabla: _**hv_precipitacion_2**_ (empty)

Tabla: _**hv_precipitacion_log_error**_ (642568)
IDEM ANTERIOR

Tabla: _**hv_precipitacion_origen**_ (24022)
- _id_
- _id_prec_
- _id_usuario_
- _id_estacion_
- _fecha_registro_
- _hora_registro_
- _mes_
- _anio_
- _lluvia_
- _nieve_
- _granizo_
- _llovizna_
- _neblina_
- _tormenta_
- _helada_
- _nrodia_
- _hora_
- _hora_ini_
- _min_ini_
- _hora_fin_
- _min_fin_
- _durac_hora_
- _durac_min_
- _cant_mm_
- _altura_
- _acumulada_
- _observ_
- _operador_
- _num_maq_
- _id_ant_

Tabla: _**hv_provincias**_ (333)
- _provinmcia_: id provincia
- _nombre_: nombre provincia
- _país_: id país

Tabla: _**hv_sessions**_ (empty)

Tabla: _**hv_timezone**_ (empty)

Tabla: _**hv_user**_ (11)
- id 	auth 	confirmed 	deleted 	username 	password 	idnumber 	firstname 	lastname 	email 	icq 	phone1 	address 	city 	country 	firstaccess 	lastaccess 	lastlogin 	currentlogin 	lastIP 	picture 	description 	timemodified

Tabla: _**hv_user_admins**_ (1) Quién es el admin (id, usr_id)

Tabla: _**hv_user_preferences**_ (2) preopiedades del usuario

Tabla: _**hv_variables**_ (35)
- _id_: identificación
- _nom_var_: nombre de la variable
- _nom_corto_: short name
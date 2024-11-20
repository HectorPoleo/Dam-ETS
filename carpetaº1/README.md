|  Actor | Cliente |
|---|---|
| Descripción  | _Acude a VIDEOMAX por diversos casos_  |
| Características  | _Puede proporcionar datos personales, al dar sus datos se registra, puede alquilar una Pelicula, puede reservar una Pelicula.  _ |
| Relaciones | __  |
| Referencias | _Una vez alquilada debe seleccionar cual quiere alquilar, una vez alquilada debe devolverla en el plazo, al alquilar se registra el alquiler, se registra la reserva. _ |   
|  Notas |  _Notas adicionales_ |
| Autor  | _HectorPoleo_ |
|Fecha | _18/11/2024_ |

|  Atributo |||
|---|---|---|
| _Nombre_  | _Descripción_  | _Tipo_ |
| | |

|  Actor | Proveedor |
|---|---|
| Descripción  | _Provee de peliculas a VIDEOMAX_  |
| Características  | _Abastece Peliculas segun sus existencias.  _ |
| Relaciones | _Administrador VIDEOMAX, le re-abastece las peliculas_  |
| Referencias | _Puede abastecer Peliculas, registra las peliculas . _ |   
|  Notas |  _Notas adicionales_ |
| Autor  | _HectorPoleo_ |
|Fecha | _18/11/2024_ |

|  Atributo |||
|---|---|---|
| _Nombre_  | _Descripción_  | _Tipo_ |
| | |

|  Actor | Administrador VIDEOMAX |
|---|---|
| Descripción  | _Administra la tienda_  |
| Características  | _Registra al cliente, registra el alquiler de la pelicula, registra la reserva de la pelicula, registra la pelicula re-abastecida.  _ |
| Relaciones | __  |
| Referencias | _Actualiza el proveedor. _ |   
|  Notas |  _Notas adicionales_ |
| Autor  | _HectorPoleo_ |
|Fecha | _18/11/2024_ |

|  Atributo |||
|---|---|---|
| _Nombre_  | _Descripción_  | _Tipo_ |
| | |

|  Caso de Uso CU | Proporcionar Datos Personales |
|---|---|
| Fuentes | _Documentos de especificaciones del sistema de registro de clientes._ |
| Actor | _Cliente_ |
| Descripción | _El cliente proporciona sus datos personales para registrarse en el sistema._ |
| Flujo básico | 1. El cliente accede a la interfaz de registro. <br> 2. El cliente ingresa sus datos personales. <br> 3. El sistema valida los datos ingresados. <br> 4. El sistema confirma la recepción de los datos. |
| Pre-condiciones | _El cliente no debe estar registrado previamente en el sistema._ |
| Post-condiciones | _El cliente ha registrado sus datos personales en el sistema._ |
| Requerimientos | _Acceso al sistema, conexión a internet._ |
| Notas | _El cliente debe completar todos los campos obligatorios._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |

|  Caso de Uso CU | Registrar al Cliente |
|---|---|
| Fuentes | _Documentos de especificaciones del sistema de registro._ |
| Actor | _Sistema, Cliente_ |
| Descripción | _Una vez que el cliente proporciona sus datos, el sistema lo registra como usuario del servicio._ |
| Flujo básico | 1. El sistema recibe los datos personales del cliente. <br> 2. El sistema verifica que los datos sean válidos. <br> 3. El sistema registra al cliente en la base de datos. <br> 4. El sistema confirma el registro exitoso al cliente. |
| Pre-condiciones | _El cliente debe haber proporcionado todos sus datos personales._ |
| Post-condiciones | _El cliente está registrado en el sistema y puede realizar transacciones._ |
| Requerimientos | _Sistema de base de datos de clientes._ |
| Notas | _El sistema debe verificar que no haya registros duplicados._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |

|  Caso de Uso CU | Alquilar una Película |
|---|---|
| Fuentes | _Documentos de especificación de alquiler de películas._ |
| Actor | _Cliente_ |
| Descripción | _El cliente selecciona y alquila una película del catálogo disponible._ |
| Flujo básico | 1. El cliente accede al catálogo de películas. <br> 2. El cliente selecciona la película que desea alquilar. <br> 3. El sistema verifica la disponibilidad de la película. <br> 4. El cliente confirma el alquiler. <br> 5. El sistema registra el alquiler y proporciona el plazo de devolución. |
| Pre-condiciones | _El cliente debe estar registrado en el sistema._ |
| Post-condiciones | _El cliente tiene un alquiler activo registrado en el sistema._ |
| Requerimientos | _Sistema de gestión de alquileres._ |
| Notas | _La película debe estar disponible para alquiler antes de que el cliente pueda alquilarla._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |

|  Caso de Uso CU | Reservar una Película |
|---|---|
| Fuentes | _Documentos de especificación de reservas de películas._ |
| Actor | _Cliente_ |
| Descripción | _El cliente puede reservar una película para alquilarla en el futuro._ |
| Flujo básico | 1. El cliente accede al catálogo de películas. <br> 2. El cliente selecciona la película que desea reservar. <br> 3. El sistema verifica la disponibilidad para la reserva. <br> 4. El cliente confirma la reserva. <br> 5. El sistema registra la reserva y proporciona el plazo para recoger la película. |
| Pre-condiciones | _El cliente debe estar registrado en el sistema._ |
| Post-condiciones | _El sistema registra la reserva de la película para el cliente._ |
| Requerimientos | _Sistema de gestión de reservas._ |
| Notas | _El cliente debe recoger la película dentro del plazo establecido._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |


|  Caso de Uso CU | Abastecer Películas según sus Existencias |
|---|---|
| Fuentes | _Documentos de especificación de abastecimiento de inventario._ |
| Actor | _Proveedor de películas_ |
| Descripción | _El proveedor abastece el inventario con películas según las existencias y la demanda._ |
| Flujo básico | 1. El proveedor accede a la lista de películas que necesitan ser abastecidas. <br> 2. El proveedor realiza el pedido de las películas faltantes. <br> 3. El sistema actualiza el inventario con las nuevas existencias. |
| Pre-condiciones | _El sistema debe tener un seguimiento de las existencias de películas._ |
| Post-condiciones | _El inventario de películas está actualizado con las nuevas existencias._ |
| Requerimientos | _Acceso al inventario, conexión a proveedores._ |
| Notas | _El sistema debe alertar al proveedor cuando una película esté baja en existencias._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |

|  Caso de Uso CU | Registrar el Alquiler de la Película |
|---|---|
| Fuentes | _Documentos de especificación del sistema de alquiler._ |
| Actor | _Sistema, Cliente_ |
| Descripción | _El sistema registra los detalles del alquiler de la película realizada por el cliente._ |
| Flujo básico | 1. El cliente confirma el alquiler de la película. <br> 2. El sistema verifica que la película esté disponible. <br> 3. El sistema registra el alquiler en la base de datos. <br> 4. El sistema genera un recibo con la fecha de devolución. |
| Pre-condiciones | _El cliente debe estar registrado y la película debe estar disponible._ |
| Post-condiciones | _El alquiler de la película se ha registrado en el sistema._ |
| Requerimientos | _Sistema de gestión de alquileres._ |
| Notas | _El alquiler debe incluir un plazo de devolución y una posible tarifa._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |

|  Caso de Uso CU | Registrar la Reserva de la Película |
|---|---|
| Fuentes | _Documentos de especificación del sistema de reservas._ |
| Actor | _Sistema, Cliente_ |
| Descripción | _El sistema registra los detalles de la reserva de la película realizada por el cliente._ |
| Flujo básico | 1. El cliente realiza una reserva de la película. <br> 2. El sistema verifica la disponibilidad de la película para la reserva. <br> 3. El sistema registra la reserva en la base de datos. |
| Pre-condiciones | _El cliente debe estar registrado y la película debe estar disponible para reserva._ |
| Post-condiciones | _La reserva ha sido registrada en el sistema._ |
| Requerimientos | _Sistema de gestión de reservas._ |
| Notas | _El cliente debe recoger la película dentro de un plazo establecido._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |


|  Caso de Uso CU | Registrar la Película Re-abastecida |
|---|---|
| Fuentes | _Documentos de especificación del sistema de inventarios._ |
| Actor | _Proveedor de películas, Sistema_ |
| Descripción | _El sistema registra las películas re-abastecidas cuando se actualizan las existencias._ |
| Flujo básico | 1. El proveedor actualiza las existencias del sistema. <br> 2. El sistema registra la película re-abastecida en el inventario. |
| Pre-condiciones | _El sistema debe tener un inventario de películas y el proveedor debe tener existencias disponibles._ |
| Post-condiciones | _El inventario ha sido actualizado con las películas re-abastecidas._ |
| Requerimientos | _Sistema de gestión de inventarios._ |
| Notas | _El sistema debe reflejar las películas re-abastecidas en tiempo real._ |
| Autor | _HectorPoleo_ |
| Fecha | _18/11/2024_ |

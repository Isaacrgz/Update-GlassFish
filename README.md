# Actualizar GlassFish Server
> [!NOTE]
> Conoce que si ya tienes aplicaciones, conexiones a bases de datos, y configuraciones en producción, puedes actulizar GlassFish Server sin tener que desplegar y configurar de nuevo.

## Pasos a seguir 
> [!WARNING]
> Si aun no cuentas con la última versión de GlassFish puedes descargarla [AQUI](https://glassfish.org/download.html).
1. Ubicate en la carpeta donde tienes intalado la *versión actual*.
> Ruta de ejemplo: C:/My-PC/ServerGF
2. Descomplime el archivo **ZIP** con la *nueva versión*, quedando las dos versiones.
> Ruta de la *versión actual*: C:/My-PC/ServerGF/glassfish-7.0.12
> 
> Ruta de la *nueva versión*: C:/My-PC/ServerGF/glassfish-7.0.14
3. Apaga el servidor con la versión actual (la más antigua).
> [!CAUTION]
> Si GlassFish Server esta como un Servicio de Windows, debes detener el servicio en lugar de apagar manualmente (asadmin.bat o admin GUI).

> [!TIP]
> Es recomendable retirar los Logs del dominio para respaldo y mantener el order.
4. Reemplaza la carpeta **domain1** de la *nueva versión* por la carpeta **domain1** de la *versión actual*.   
> C:/My-PC/ServerGF/glassfish-7.0.14/glassfish7/glassfish/domains/domain1 en C:/My-PC/ServerGF/glassfish-7.0.14/glassfish7/glassfish/domains/domain1
5. Inicia manualmente GlassFish Server para comprobar que las aplicaciones, conexiones y configuraciones esten correstas.

6. Si todo funciona adecuadamente, puedes continuar con Eliminar el servicio de glassfish de la versión antigua.
 
7. Instala GlassFish Server como [Servicio de Windows](https://github.com/Isaacrgz/Glassfish-as-a-Windows-Service/blob/main/README.md) para la nueva versión.

# Otras ayudas de GlassFish Server
   - [Iniciar y apagar manualmente GlassFish](https://github.com/Isaacrgz/Start-Glassfish/blob/main/README.md)
   - [GlassFish Server como servicio de Windows](https://github.com/Isaacrgz/Glassfish-as-a-Windows-Service/blob/main/README.md)

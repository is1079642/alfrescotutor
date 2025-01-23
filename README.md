# Curso Práctico de Alfresco

---

## Objetivo del Curso

- Brindar conocimientos prácticos sobre administración básica de Alfresco
- Incluye:
  - Inicio y parada de servicios
  - Ubicación de archivos clave
  - Resolución de problemas comunes

---

## Inicio y Parada de Servicios

### Comandos Básicos

- Iniciar Alfresco:
  ```
  sudo systemctl start alfresco
  ```

- Detener Alfresco:
  ```
  sudo systemctl stop alfresco
  ```

- Reiniciar Alfresco:
  ```
  sudo systemctl restart alfresco
  ```

- Verificar estado:
  ```
  sudo systemctl status alfresco
  ```

---

## Servicios Relacionados

### Parada de Servicios
- solr
- tomcat
- transform
- activemq

### Inicio de Servicios
- activemq
- transform
- tomcat
- solr

---

## Ubicación de Archivos Importantes

### Archivo de Configuración
- Nombre: `alfresco-global.properties`
- Ubicación: `/opt/alfresco-content-services-7.2/apache-tomcat-9.0.62/shared/classes`

### Directorio de Logs
- Ubicación: `/opt/alfresco-content-services-7.2/apache-tomcat-9.0.62/logs/`

Logs importantes:
- `catalina.out`: Eventos de Tomcat
- `alfresco.log`: Actividades del repositorio
- `hs_err_pid*`: Diagnósticos de bloqueos Java
- `localhost_access_log*`: Solicitudes web
- `share.log.*`: Actividades en Alfresco Share

---

## Resolución de Problemas Comunes

### Revisión de Logs en Tiempo Real
```
tail -f /opt/alfresco-content-services-7.2/apache-tomcat-9.0.62/logs/alfresco.log
```

### Monitoreo del Sistema

Comandos útiles:
- `top`: Uso de recursos
- `df -h`: Espacio en disco
- `free -h`: Memoria del sistema

---

## Directorio alf_data

- Ubicación: `/opt/alfresco-content-services-7.2/alf_data`
- Contiene datos principales de Alfresco
- Verificar tamaño:
  ```
  du -sh /opt/alfresco-content-services-7.2/alf_data
  ```

---

## Conclusión

### Aspectos Cubiertos
- Inicio y parada de servicios
- Ubicación de archivos clave
- Técnicas básicas de resolución de problemas

### Próximos Pasos
- Aprender configuración avanzada
- Profundizar en administración de Alfresco

---

## Preguntas
¿Alguna duda o consulta?

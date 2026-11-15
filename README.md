# PC Doctor · lista de bloqueo

Este repositorio es **público a propósito**: las apps de PC Doctor leen de aquí
`bloqueos.json` para saber si deben bloquearse en un equipo.

- La lista va **firmada** con la llave del propietario: nadie más puede crear una válida,
  y las apps rechazan cualquier cambio que no venga de esa llave.
- No contiene datos personales: los nicknames van como huellas (resúmenes), los equipos
  como un ID anónimo y las claves revocadas por su número de serie.

## Cómo actualizarla (propietario)

1. En **PC-Doctor-Admin**, apartado *Llaves de invitación* → *Bloquear la app*, marca lo
   que quieras y pulsa **Firmar y guardar lista** → **Copiar lista firmada**.
2. Abre [`bloqueos.json` para editarlo](../../edit/main/bloqueos.json), borra todo, pega y
   pulsa **Commit changes**.
3. Las apps la leen al abrirse y cada 6 horas.

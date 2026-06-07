# SX12 no conecta por Wi-Fi después de actualizar a firmware S2.8.x (Instrument Password)

## Diagnóstico rápido

Si se cumplen las siguientes condiciones:

* Estación total Trimble SX12 con firmware **S2.8.x o superior**
* Controlador TSC7 (u otro compatible)
* Trimble Access **anterior a la versión 2023.00**
* Conexión mediante **Wi-Fi** o **Wi-Fi HaLow**

es posible que el controlador no pueda conectarse al instrumento debido a una incompatibilidad con la nueva función de **Contraseña de Instrumento** (Instrument Password).

La solución consiste en actualizar Trimble Access a la versión **2023.00 o posterior**.

---

## Síntomas

Los siguientes comportamientos pueden indicar este problema:

* La SX12 aparece en la lista de redes Wi-Fi disponibles.
* El controlador se conecta correctamente a la red inalámbrica de la SX12.
* Trimble Access no logra establecer conexión con el instrumento.
* La conexión falla o expira después de varios intentos.
* El software no solicita ninguna contraseña de instrumento.
* El problema aparece inmediatamente después de actualizar el firmware de la SX12.

En muchos casos, el problema puede confundirse con una falla de red, una configuración incorrecta de Wi-Fi o un problema de hardware.

---

## Causa

A partir del firmware **S2.8.x**, el Trimble SX12 incorpora una función de seguridad denominada **Contraseña de Instrumento** para las conexiones mediante Wi-Fi y Wi-Fi HaLow.

Cuando una SX12 actualizada a S2.8.x o superior recibe su primera conexión, Trimble Access solicita configurar una contraseña que posteriormente será almacenada tanto en el instrumento como en el controlador. Mientras ambas contraseñas coincidan, las conexiones futuras se realizarán automáticamente.

Las versiones antiguas de Trimble Access no incluyen soporte para esta funcionalidad y, por lo tanto, no pueden gestionar correctamente el proceso de autenticación requerido por el nuevo firmware.

---

## Configuraciones afectadas

| Componente         | Versión                           |
| ------------------ | --------------------------------- |
| Instrumento        | SX12 firmware S2.8.x o superior   |
| Software           | Trimble Access anterior a 2023.00 |
| Método de conexión | Wi-Fi o Wi-Fi HaLow               |

---

### Actualizar Trimble Access

La solución recomendada es actualizar Trimble Access a la versión **2023.00 o posterior**.

Trimble incorporó oficialmente el soporte para Contraseña de Instrumento de la SX12 en la versión 2023.00.

Después de la actualización:

1. Conecte el controlador a la SX12.
2. Ingrese la contraseña del instrumento cuando se le solicite.
3. Si corresponde, reemplace la contraseña predeterminada de fábrica por una nueva contraseña.
4. Espere a que la contraseña se almacene en el instrumento y en el controlador.
5. Verifique que la conexión se establezca correctamente.

---

## Verificación

Para confirmar si este diagnóstico aplica:

### En el SX12

Verificar la versión de firmware instalada.

Si la versión es:

```text
S2.8.x o superior
```

continuar con la siguiente comprobación.

### En el controlador

Verificar la versión de Trimble Access instalada.

Si la versión es:

```text
Anterior a 2023.00
```

existe una alta probabilidad de que la causa del problema sea la falta de soporte para Contraseña de Instrumento.

---

## Referencias

* [Notas de versión de Trimble Access 2023.00](https://help.fieldsystems.trimble.com/trimble-access-release-notes/en/2023.00.htm).
* [Contraseña de Instrumento para SX12](https://help.fieldsystems.trimble.com/trimble-access/latest/en/instrument-password.htm).

# mmnetguard-config

Configuración remota **firmada** de MM NetGuard.

La app de control (`MMNetGuard.Control.exe`, en la PC del administrador) publica
aquí el archivo **`netguard.json`**, firmado con ECDSA. La PC destino lo baja por
su URL cruda y verifica la firma con la llave pública antes de aplicarlo. Sin la
llave privada nadie puede falsificar la configuración.

**No pongas nada sensible aquí** (no va contraseña): solo el horario, el
interruptor maestro, el desbloqueo temporal y el corte total.

URL cruda que usa la PC destino:

```
https://raw.githubusercontent.com/mirangerardo-code/mmnetguard-config/main/netguard.json
```

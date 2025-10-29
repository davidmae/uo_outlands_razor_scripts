# Scripts de Razor para UO Outlands

## Scripts de Attack + Hiding

Esta colección incluye tres scripts diferentes para atacar y activar Hiding en UO Outlands.

---

## 📜 Scripts Incluidos

### 1. **attack_and_hide.razor** - Básico
Script simple que ataca una vez y activa Hiding.

**Uso:**
1. Establece un objetivo (haz clic derecho > Set Last Target o usa un hotkey)
2. Ejecuta el script
3. El personaje atacará y luego se ocultará

**Ideal para:**
- Ataques rápidos en PvP
- Hit and run
- Entrenamientos básicos

---

### 2. **attack_hide_loop.razor** - Loop Continuo
Script con loop infinito que ataca y se esconde repetidamente.

**Uso:**
1. Establece un objetivo
2. Ejecuta el script
3. El script continuará en loop hasta que lo detengas manualmente
4. Para detener: presiona el botón "Stop Macro" en Razor

**Ideal para:**
- Entrenamiento de Hiding skill
- Farming con stealth
- Combate prolongado con táctica de hit and run

**Nota:** El script espera 10 segundos entre cada ciclo (cooldown de Hiding)

---

### 3. **smart_attack_hide.razor** - Inteligente
Script avanzado con verificaciones de seguridad.

**Características:**
- Verifica tu salud antes de atacar (se detiene si HP < 30)
- Detecta si el objetivo fue eliminado
- Confirma si el Hiding fue exitoso
- Mensajes visuales de estado

**Uso:**
1. Establece un objetivo
2. Ejecuta el script
3. El script verificará condiciones y ejecutará el ataque + hiding

**Ideal para:**
- PvP donde necesitas monitorear tu salud
- Situaciones donde necesitas confirmación visual
- Uso general más seguro

---

## ⚙️ Instalación

1. Copia el archivo .razor que desees usar
2. En Razor, ve a la pestaña de **Macros**
3. Haz clic en **New** para crear una nueva macro
4. Haz clic en **Open** y selecciona el archivo .razor
5. Asigna un hotkey a la macro si lo deseas

---

## 🎮 Configuración Recomendada

### Requisitos:
- **Hiding skill**: Necesitas tener la habilidad Hiding en tu personaje
- **Target establecido**: Debes tener un objetivo establecido antes de ejecutar el script

### Hotkeys Recomendados:
- `Tab`: Set Last Target
- `F1-F4`: Tus scripts de attack + hide
- `Esc`: Stop All Macros (emergencia)

---

## 🔧 Personalización

Puedes modificar los scripts según tus necesidades:

### Cambiar tiempos de espera:
```
pause 250  // Cambia este valor (en milisegundos)
```

### Cambiar umbral de salud (smart_attack_hide.razor):
```
if hp < 30  // Cambia 30 al valor de HP que prefieras
```

### Cambiar cooldown del loop (attack_hide_loop.razor):
```
pause 10000  // 10 segundos, ajusta según tu cooldown
```

### Cambiar colores de mensajes:
Los números al final de `overhead` son códigos de color:
- `88`: Verde (éxito)
- `33`: Rojo (error/advertencia)
- `58`: Amarillo (información)

---

## 💡 Tips y Consejos

1. **Entrenamiento de Hiding:**
   - Usa `attack_hide_loop.razor`
   - Ataca a un NPC pacífico o a un dummy
   - Ajusta el cooldown según tu skill level

2. **PvP:**
   - Usa `smart_attack_hide.razor` para mayor seguridad
   - Combina con pociones de invisibilidad como backup
   - Practica el timing en áreas seguras primero

3. **Farming:**
   - `attack_and_hide.razor` es ideal para mobs individuales
   - Combina con scripts de looting para eficiencia

4. **Debug:**
   - Si el Hiding falla constantemente, verifica:
     - Que no estés en combate muy activo
     - Tu skill level de Hiding
     - Que no tengas el status "Recently Hidden"

---

## ⚠️ Advertencias

- **No uses scripts AFK** - Contra las reglas del servidor
- **Verifica las reglas del servidor** sobre automatización
- **Los scripts son herramientas**, úsalos responsablemente
- **Siempre mantén control manual** para emergencias

---

## 🤝 Contribuciones

¿Tienes mejoras o nuevos scripts? ¡Siéntete libre de contribuir!

---

## 📝 Notas de Versión

**v1.0** - Lanzamiento inicial
- Script básico de attack + hide
- Script con loop continuo
- Script inteligente con verificaciones

---

**¡Feliz hunting en UO Outlands!** 🗡️🌙

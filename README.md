# ⚡ iAxCrystalOptimizer

> **Place Crystals at the speed of light.**

A fork of the WalksyCrystal mod for Minecraft Fabric. It improves the placement and destruction speed of End Crystals, designed for PvP Crystal players seeking maximum speed.

[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.1--1.21.4-brightgreen.svg)](https://www.minecraft.net/)
[![Fabric](https://img.shields.io/badge/Fabric-0.16.0+-orange.svg)](https://fabricmc.net/)
[![Java](https://img.shields.io/badge/Java-21+-blue.svg)](https://www.oracle.com/java/)

---

## 📋 Características

### 🚀 Optimización de Cristales
- **Colocación Ultra-Rápida**: Coloca cristales de End a velocidades optimizadas
- **Destrucción Mejorada**: Rompe cristales con latencia mínima
- **Sistema Anti-Detección**: Implementa cooldowns adaptativos y variación aleatoria para evitar patrones detectables
- **Límite Adaptativo de Paquetes**: Ajusta automáticamente el límite de paquetes basándose en tu ping

### ⚙️ Sistema de Configuración
- **Múltiples Modos**: Vanilla, Legit, Balanced, Aggressive, Custom
- **Configuración Personalizable**: Ajusta cooldowns de colocación y destrucción según tus necesidades
- **Comandos en el Juego**: Activa/desactiva el optimizador con comandos simples
- **Integración con MidnightLib**: Interfaz de configuración intuitiva

### 🎯 Características Técnicas
- **Verificación del Lado del Servidor**: Validación adecuada para evitar desincronización
- **Optimización de Raycast**: Detección precisa de bloques y entidades
- **Soporte Multi-Entidad**: Compatible con End Crystals, Slimes y Magma Cubes
- **Cooldown Inteligente**: Sistema de cooldown que previene spam excesivo

---

## 📦 Instalación

### Requisitos Previos
- **Minecraft**: 1.21.1 - 1.21.4
- **Fabric Loader**: 0.16.0 o superior
- **Java**: 21 o superior
- **Fabric API**: Última versión
- **MidnightLib**: Última versión

### Pasos de Instalación

1. **Descarga el Mod**
   - Ve a la sección [Releases](https://github.com/iAkcc/iAxCrystalOptimizer/releases)
   - Descarga el archivo `.jar` más reciente

2. **Instala las Dependencias**
   - Descarga [Fabric API](https://modrinth.com/mod/fabric-api)
   - Descarga [MidnightLib](https://modrinth.com/mod/midnightlib)

3. **Coloca los Archivos**
   - Abre tu carpeta `.minecraft/mods`
   - Coloca `iaxcrystaloptimizer-1.4.0.jar`, Fabric API y MidnightLib en la carpeta

4. **Inicia Minecraft**
   - Selecciona el perfil de Fabric
   - ¡Disfruta del mod!

---

## 🎮 Uso

### Comandos Disponibles

```
/optimizer toggle - Activa/desactiva el optimizador
/optimizer enable - Activa el optimizador
/optimizer disable - Desactiva el optimizador
```

### Modos de Configuración

| Modo | Cooldown Colocación | Cooldown Destrucción | Descripción |
|------|---------------------|----------------------|-------------|
| **Vanilla** | 250ms | 250ms | Comportamiento vanilla de Minecraft |
| **Legit** | 100ms | 100ms | Mejora sutil, difícil de detectar |
| **Balanced** | 50ms | 50ms | Balance entre rendimiento y legitimidad |
| **Aggressive** | 25ms | 25ms | Máximo rendimiento (más detectable) |
| **Custom** | Personalizado | Personalizado | Define tus propios valores |

### Controles

- **Clic Derecho** (con cristal en mano): Coloca cristales optimizados en obsidiana/bedrock
- **Clic Izquierdo** (mirando a un cristal): Destruye cristales con latencia reducida

---

## 🛠️ Compilación desde el Código Fuente

### Requisitos
- JDK 21 o superior
- Git

### Pasos

```bash
# Clona el repositorio
git clone https://github.com/iAkcc/iAxCrystalOptimizer.git
cd iAxCrystalOptimizer

# Compila el proyecto
./gradlew build

# El archivo .jar estará en build/libs/
```

---

## 🔧 Configuración Técnica

### Sistema de Límite de Paquetes Adaptativo

El mod ajusta automáticamente el límite de paquetes basándose en tu ping:

```java
Ping < 50ms   → Límite: 3-4 paquetes
Ping 50-100ms → Límite: 2-3 paquetes
Ping > 100ms  → Límite: 1-2 paquetes
```

### Variación Aleatoria

Para evitar patrones detectables, el mod añade una variación aleatoria del 30% al límite de paquetes, haciendo que el comportamiento parezca más humano.

---

## 📝 Notas Importantes

> [!WARNING]
> Este mod está diseñado para uso en servidores que permiten mods del lado del cliente. **Úsalo bajo tu propio riesgo** en servidores con políticas estrictas contra mods de PvP.

> [!IMPORTANT]
> El mod implementa medidas anti-detección, pero no garantiza que sea 100% indetectable en todos los servidores. Siempre verifica las reglas del servidor antes de usar.

> [!NOTE]
> El modo "Vanilla" está diseñado para ser completamente legítimo y no debería ser detectable, ya que replica el comportamiento vanilla de Minecraft.

---

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si deseas mejorar el mod:

1. Haz un Fork del proyecto
2. Crea una rama para tu característica (`git checkout -b feature/NuevaCaracteristica`)
3. Commit tus cambios (`git commit -m 'Añadir nueva característica'`)
4. Push a la rama (`git push origin feature/NuevaCaracteristica`)
5. Abre un Pull Request

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---

## 👤 Autor

**iAxres**

- GitHub: [@iAkcc](https://github.com/iAkcc)

---

## 🙏 Agradecimientos

- **Walksy** - Por el concepto original del Crystal Optimizer
- **Fabric Team** - Por el increíble framework de modding
- **MidnightDust** - Por MidnightLib y el sistema de configuración

---

## 📊 Estadísticas del Proyecto

![GitHub stars](https://img.shields.io/github/stars/iAkcc/iAxCrystalOptimizer?style=social)
![GitHub forks](https://img.shields.io/github/forks/iAkcc/iAxCrystalOptimizer?style=social)
![GitHub issues](https://img.shields.io/github/issues/iAkcc/iAxCrystalOptimizer)

---

<div align="center">

**⚡ Hecho con ❤️ por iAxres**

*"Place Crystals at the speed of light."*

</div>

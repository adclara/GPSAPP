# 📏 Guía Rápida: Medición de Altura

## Métodos Disponibles

### ✅ Método 1: Distancia Conocida (Más Simple)

**Cuando usar:**
- Sabes o puedes medir la distancia horizontal al objetivo
- Medición de un solo punto
- Más rápido y directo

**Pasos:**
1. **Mide o estima la distancia horizontal** al objetivo (en pies)
2. **Ingresa tu altura de instrumento** (altura desde el suelo hasta tus ojos/teléfono)
   - Por defecto: 5.5 ft (persona promedio sosteniendo teléfono)
   - Ajusta según tu altura o si usas trípode
3. **Ingresa la distancia horizontal** en el campo correspondiente
4. **Apunta con el crosshair** a la parte superior del objetivo
5. **Presiona "🎯 Calcular Altura"**

**Resultados:**
- **Altura Objetivo**: Altura total del objeto desde el suelo
- **Diferencia**: Diferencia de altura respecto a tu instrumento

**Ejemplo:**
```
Instrumento: 5.5 ft (tu altura de ojos)
Distancia: 50 ft (al edificio)
Ángulo vertical: +30° (apuntando arriba)

Resultado: Edificio de 34' 5" de altura
```

---

### ✅ Método 2: Dos Estaciones (Sin Medir Distancia)

**Cuando usar:**
- No puedes medir la distancia al objetivo
- Objetivo inaccesible (río, barranco, etc.)
- Máxima precisión profesional

**Pasos:**
1. **Estación 1:**
   - Ingresa altura de instrumento
   - Apunta al objetivo (parte superior)
   - Presiona "🎯 Calcular Altura"
   - App guarda Punto 1 con GPS

2. **Muévete a Estación 2:**
   - Camina 50-100 ft perpendicular o hacia/desde el objetivo
   - El GPS registra tu nueva posición automáticamente
   - Mantén misma altura de instrumento

3. **Estación 2:**
   - Apunta al MISMO punto del objetivo
   - Presiona "🎯 Calcular Altura" de nuevo
   - App calcula usando triangulación

**Resultados:**
- **Altura Objetivo**: Calculada por triangulación
- **Diferencia**: Desde tu instrumento
- **Dist. Calculada**: Distancia de Estación 1 al objetivo

**Ejemplo:**
```
Estación 1: Lat 26.1234, Lon -80.5678
Ángulo vertical: +25°
Instrumento: 5.5 ft

[Caminas 75 ft]

Estación 2: Lat 26.1240, Lon -80.5682
Ángulo vertical: +18°
Instrumento: 5.5 ft

Resultado: 
- Altura: 42' 3"
- Distancia calculada: 120 ft
```

---

## 💡 Tips Profesionales

### Altura de Instrumento
- **Persona de pie**: 5.0 - 6.0 ft (depende de tu estatura)
- **Con trípode bajo**: 3.5 - 4.5 ft
- **Con trípode estándar**: 4.5 - 5.5 ft
- **Sentado/arrodillado**: 2.5 - 3.5 ft

**Medir exactamente:**
1. Párate en posición de medición
2. Otra persona mide desde el suelo hasta tus ojos/teléfono
3. O usa cinta métrica contra pared

### Mejores Prácticas

**✅ HAZ:**
- Nivela el instrumento (burbujas centradas)
- Usa trípode para mayor estabilidad
- Mide distancias con cinta métrica cuando sea posible
- Toma múltiples mediciones y promedia
- Verifica GPS tiene buena señal (<33 ft de precisión)
- Anota condiciones (viento, temperatura)

**❌ NO HAGAS:**
- Medir con viento fuerte
- Usar en lluvia o niebla
- Medir con sol directo en pantalla
- Cambiar altura de instrumento entre estaciones
- Moverte durante la medición
- Confiar en distancias estimadas a ojo

### Precisión Esperada

**Método 1 (Distancia Conocida):**
- Con distancia exacta: ±1-2 ft
- Con distancia estimada: ±5-10 ft
- Depende de: precisión de distancia, nivelación, ángulo vertical

**Método 2 (Dos Estaciones):**
- Con GPS preciso: ±2-4 ft
- Con GPS regular: ±5-8 ft
- Depende de: precisión GPS, distancia entre estaciones, ángulos

---

## 🎯 Casos de Uso Comunes

### 1. Altura de Edificio
**Mejor método:** Método 1
- Mide distancia con cinta métrica
- Párate a distancia conocida
- Apunta a la parte superior

### 2. Altura de Árbol en Bosque
**Mejor método:** Método 2
- No puedes acercarte para medir
- Dos estaciones dan resultado sin medir

### 3. Altura de Poste de Luz
**Mejor método:** Método 1
- Fácil medir distancia
- Objetivo pequeño, apuntar es fácil

### 4. Acantilado o Barranco
**Mejor método:** Método 2
- Imposible medir distancia
- Dos ángulos desde ubicaciones seguras

### 5. Verificación de Elevación de Construcción
**Mejor método:** Método 1
- Puedes usar cinta métrica
- Necesitas precisión

---

## 📋 Checklist de Medición

Antes de medir:
- [ ] GPS tiene señal (<33 ft de precisión)
- [ ] Burbujas de nivel centradas
- [ ] Altura de instrumento ingresada correctamente
- [ ] Crosshair visible y estable
- [ ] Clima apropiado (sin lluvia/viento fuerte)

Durante medición:
- [ ] Teléfono estable (usar trípode si es posible)
- [ ] Crosshair apunta exactamente al objetivo
- [ ] Ángulo vertical se muestra estable
- [ ] No hay obstáculos en línea de visión

Después de medir:
- [ ] Resultado tiene sentido (comparar con estimación)
- [ ] Captura medición (botón 📍) para guardar
- [ ] Anota condiciones especiales
- [ ] Toma foto de referencia si es posible

---

## 🔧 Solución de Problemas

**"Resultado no tiene sentido"**
- Verifica altura de instrumento
- Confirma distancia ingresada
- Revisa que burbujas estén centradas
- Asegúrate de apuntar al punto correcto

**"Método 2 dice 'activa GPS'"**
- Verifica permisos de ubicación
- Espera señal GPS (indicador arriba)
- Muévete a área abierta

**"Altura negativa"**
- Normal si objetivo está debajo de ti
- Verifica ángulo vertical (debe ser negativo)

**"Diferencia entre mediciones"**
- Toma 3-5 mediciones
- Promedia los resultados
- Descarta valores extremos
- Considera condiciones (viento, movimiento)

---

## 📐 Fórmulas Utilizadas

### Método 1 (Distancia Conocida)
```
Diferencia_Altura = Distancia_Horizontal × tan(Ángulo_Vertical)
Altura_Objetivo = Altura_Instrumento + Diferencia_Altura
```

### Método 2 (Dos Estaciones)
```
Usa trigonometría avanzada con:
- Distancia entre estaciones (GPS)
- Ángulo desde Estación 1
- Ángulo desde Estación 2
- Ley de senos para triangulación
```

---

## 💾 Exportar Datos

Todas las mediciones de altura se guardan con:
- Timestamp
- Ángulos (Hz, V, Z)
- GPS coordinates
- Altura de instrumento
- Distancia horizontal (si usaste)
- **Altura objetivo calculada**
- **Diferencia de altura**

Exporta a CSV desde el menú 📋 para análisis posterior.

---

**Nota:** Este teodolito digital es excelente para mediciones preliminares y educativas. Para trabajos de ingeniería críticos o legales, siempre verifica con equipo profesional.

**¡Buena medición!** 🎯📏

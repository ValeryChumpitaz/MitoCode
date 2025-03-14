# 🐾 Pruebas Unitarias con Mockito - Registro de Mascotas  

Este repositorio contiene pruebas unitarias para el servicio de registro de mascotas utilizando **JUnit 5 y Mockito**. La finalidad es asegurar que el registro de mascotas se realice correctamente y sin errores, evitando dependencias reales.  

## 🚀 Tecnologías Utilizadas  
✅ **Java 17**  
✅ **JUnit 5** - Framework de testing  
✅ **Mockito** - Mocking de dependencias  
✅ **Maven** - Gestión de dependencias  

---

## 📌 Instalación y Configuración  
Para ejecutar este proyecto en tu entorno local, sigue estos pasos:  

1. **Clona el repositorio**  
   ```bash
   git clone https://github.com/tu-usuario/MitoCode.git
   cd mockito-mascotas

## 📝 Descripción de las Pruebas  

### 📌 `MascotaService01JUnit1Test.java`
Este archivo contiene pruebas unitarias para verificar que el método `registrarMascota()` funcione correctamente.  

### 🔍 Casos de Prueba  

✅ **Registro exitoso de mascota:**  
   - Se verifica que la mascota no sea `null` después de registrarla.  
   - Se comprueba que el nombre de la mascota coincida con el esperado.  

✅ **Test Placeholder (`testTrue`)**  
   - Test que simplemente valida `assertTrue(true)` para verificar que la suite de pruebas corre sin errores.  

---

## 🔥 Buenas Prácticas y Recomendaciones  

✔️ **Usar Mocks en los Servicios Dependientes:** Evita llamadas reales a la base de datos o servicios externos.  
✔️ **Verificar Interacciones con `verify()`**: Asegura que los métodos mockeados se ejecuten correctamente.  
✔️ **Utilizar `@BeforeEach` para Inicializar los Mocks:** Evita errores de inicialización.  
✔️ **Mantener los Tests Aislados:** No dependas de archivos externos ni conexiones reales.  

---

## 🚫 Errores Comunes y Qué Evitar  

❌ **No inicializar Mockito correctamente**  
   - 🔹 **Solución:** Usa `MockitoAnnotations.openMocks(this)` en `@BeforeEach`.  

❌ **No usar `@Mock` y `@InjectMocks` correctamente**  
   - `@Mock` → Crea un mock de una dependencia.  
   - `@InjectMocks` → Inyecta los mocks dentro del servicio que se está probando.  

❌ **Probar integración en vez de unidad**  
   - Estas pruebas deben enfocarse en lógica de negocio, no en base de datos ni APIs externas.  

---

## 🏆 Autor  
📌 **Este proyecto fue desarrollado por [Valery Chumpitaz](https://github.com/tu-usuario).**  
📌 Si te sirvió, **¡no olvides dejar una ⭐ en el repo!** 😎  

---

💡 **¿Mejoras o sugerencias?** ¡Siéntete libre de contribuir o hacer un pull request! 🚀  

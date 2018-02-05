# Scrum Notes

- La esencia del agilismo es la habilidad para adaptarse a los cambios
- Propiedad colectiva: El código pertenece a todo el equipoy cualquier desarrollador está en condiciones de modificr el código escrito por otro.
- Los imprevistos tiene prioridad por sobre lo planificado.
- Es recomendable utilizar patrones de diseño y otras buenas prácticas pero siempre dando máxima importancia y prioridad a los requisitos del negocio.
- La Aplicación se despliega en QA a diario de forma automatizada
- Las baterías de tests se ejecutan varias veces al dia.
- la cobertura de los test deb ser >=60%
- Push a los repos al menos una vez al dia.
- Cada nueva feature debe pasar a QA
- Code review

# Roles en SCRUM
- **Product Owner**: Pedir lo que necesita. (el Qué, **no** el cómo)
- **Cliente**: Dueño del producto y usuario final
- **Analista de Negocio**: Traduce los requisitos en **test** de aceptación, articula al **product owner** con los **Devs**
- **Devs**: Toman la información del analista y deciden **cómo** lo van a resolver e implementan la solución.
- **Sysadmin**: Mantener servidores y servicios que los **devs** necesitan

En equipos pequeños una persona puede tener mas de un rol.

# Algoritmo TDD
1. Escribir las especificaciones primero (en forma de código)
2. Implementar el código según las especificciones
3. Refactorizar

### Referencias
- [Diseño Ágil con TDD](http://www.carlosble.com/downloads/disenoAgilConTdd_ebook.pdf), carlosble

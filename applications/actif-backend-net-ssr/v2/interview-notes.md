# Notas de Entrevista - Backend Developer .NET SSR

**Empresa:** No revelada (reclutamiento vía ACTIF TalentXperts)
**Rol:** Backend Developer .NET SSR
**Ubicación:** La Plata, Buenos Aires, Argentina (Híbrido/Remoto)

---

## Acción Pre-Entrevista

Solicitar a ACTIF que revele el nombre de la empresa antes de la entrevista. Investigar la empresa una vez identificada.

---

## Investigación Mínima de la Empresa

- SaaS B2B, más de 10 años en LATAM, miles de usuarios
- Productos que incorporan IA
- Stack: C#/.NET, AWS (Lambda, S3, RDS), microservicios, arquitectura event-driven
- Híbrido/remoto desde La Plata

---

## Requisitos vs. Perfil

| Requisito | Mi Match | Punto para destacar |
|-----------|----------|---------------------|
| C# / .NET | 4+ años (SYNAgro, Eppical, La Nación) | Migración .NET en La Nación, backend C# en Eppical |
| APIs REST | Competencia central | Diseño de APIs en migración de newsletters y Paywall |
| SQL Server | Experiencia directa (Eppical, SYNAgro) | Separación de capas de BD en Eppical |
| AWS | Lambda, EventBridge, SQS, CloudWatch, CDK | Arquitectura event-driven en La Nación |
| Microservicios | Experiencia directa via monorepo + event-driven | Servicios backend con EventBridge + SQS |
| Integración con IA | Experiencia directa (Eppical) | OpenAI APIs en procesamiento documental |
| Code reviews | Práctica actual en La Nación | Azure DevOps, equipos cross-functional |
| CI/CD / Azure Pipelines | Experiencia directa | Pipelines Azure DevOps en La Nación |
| IaC (CDK/Terraform) | AWS CDK en producción | Aprovisionamiento de infraestructura en migración |
| Docker | En aprendizaje activo | Enmarcar como skill-building con base de infra |

---

## Elevator Pitch (1-2 minutos)

"Soy Software Engineer con experiencia en desarrollo backend, cloud y modernización de sistemas. En La Nación contribuí a la migración de un sistema legacy .NET 2.2 de newsletters hacia una arquitectura event-driven en Node.js y AWS, desarrollando APIs REST y servicios backend con Lambda, EventBridge y SQS, y aprovisionando infraestructura con AWS CDK. También trabajé como desarrollador core en el Paywall, colaborando con equipos de Arquitectura, Base de Datos y Frontend. Antes, en Eppical, integré OpenAI APIs en flujos de procesamiento documental y participé en la evolución de la arquitectura separando responsabilidades entre capas. Aplico principios SOLID en producción y disfruto trabajar con arquitecturas cloud y colaborar en equipos multidisciplinarios. Actualmente curso Seguridad Informática en la Universidad Siglo 21."

---

## Historias STAR

### Historia 1: Migración Legacy .NET a Node.js + AWS (La Nación)

**S:** El sistema de newsletters corría sobre .NET 2.2 con Lambdas de AWS y dependencias complejas, difícil de mantener.
**T:** Contribuir a la migración del backend a Node.js, definir la nueva arquitectura y asegurar que el sistema siguiera funcionando sin interrupciones.
**A:** Mapeé las Lambdas existentes y el flujo de datos, propuse una arquitectura event-driven con EventBridge, SQS y servicios serverless. Diseñé las APIs REST, aprovisioné infraestructura con CDK, configuré Dead Letter Queues y CloudWatch, y coordiné con el equipo de frontend para integración incremental.
**R:** Entregamos un backend event-driven en Node.js + AWS que reemplazó el stack legacy .NET, mejoró la mantenibilidad y le dio al equipo un camino claro para extender el producto.

### Historia 2: Integración de IA en Procesamiento Documental (Eppical)

**S:** Un cliente del sector seguros necesitaba procesar documentos escaneados de forma automatizada. El proceso existente era manual y propenso a errores.
**T:** Integrar análisis documental con IA para extraer información automáticamente de PDFs e imágenes.
**A:** Investigué e integré OpenAI APIs para análisis de imágenes y extracción de texto. Conecté los resultados en servicios C#/.NET y Node.js, y construí los flujos de revisión en Angular.
**R:** El cliente procesó documentos significativamente más rápido. La funcionalidad se convirtió en parte del producto core e influyó en el roadmap del equipo.

### Historia 3: Depuración de un Problema en Producción (La Nación)

**S:** Los envíos de newsletters fallaban intermitentemente. Los logs del sistema legacy .NET no tenían tracing consistente.
**T:** Identificar la causa raíz y resolver el problema sin afectar los envíos programados.
**A:** Agregué logging estructurado y correlation IDs. Trazé los eventos a través de EventBridge y analicé los logs de ejecución de Lambda en CloudWatch. Identifiqué un timeout en la llamada a un proveedor externo de email. Implementé reintentos con exponential backoff y una Dead Letter Queue.
**R:** El problema se volvió trazable y recuperable automáticamente. Redujimos los envíos fallidos y el equipo ganó visibilidad sobre todo el flujo.

---

## Preguntas de Comportamiento

### "¿Por qué este rol?"

"Este rol combina lo que ya hago bien — desarrollo backend en .NET y AWS — con lo que quiero profundizar: microservicios, arquitecturas event-driven y productos SaaS que usan IA. Mi experiencia en la migración de La Nación con EventBridge, SQS y CDK es directamente aplicable al tipo de sistemas que describen en la búsqueda."

### "¿Dónde te ves en 3 a 5 años?"

"Quiero crecer como backend engineer especializado en cloud y arquitecturas distribuidas, combinando diseño de sistemas con IA e ingeniería de datos. Este rol me daría profundidad en microservicios, event-driven y cloud-native, que es exactamente la base que necesito."

### "¿Cómo manejás requisitos ambiguos?"

"Pregunto directo y documento las respuestas. En La Nación, la migración de newsletters arrancó con un brief vago. Mapeé el sistema existente, clarifiqué qué significaba éxito, propuse fases y alineé expectativas antes de escribir código. Prefiero surfear incertidumbre temprano que construir lo incorrecto."

### "Contame de una vez que no estuviste de acuerdo con una decisión técnica."

"Me enfoco en evidencia. Si creo que otro enfoque funciona mejor, llevo datos o un prototipo. En La Nación, cuando discutíamos cómo estructurar los servicios del Paywall, propuse un diseño modular y mostré cómo reducía el acoplamiento. Si el equipo decide otro camino después de discutirlo, me comprometo completamente con la decisión."

---

## Cómo Abordar los Gaps

**Docker:** "Tengo conocimiento práctico de proyectos personales y estoy construyendo experiencia más profunda. Mi trabajo con CDK me da una base sólida de infraestructura que acelera la curva de aprendizaje en contenedores."

**Inglés B1:** "Leo documentación técnica en inglés a diario y participo en reuniones en inglés cuando es necesario. Mi inglés técnico es sólido; la fluidez conversacional es mi foco actual de mejora."

---

## Preguntas para el Entrevistador

- ¿Cómo está estructurado el equipo de ingeniería? ¿Con quiénes trabajaría más de cerca?
- ¿Qué tan integrada está la IA en los productos actuales? ¿Qué rol juega el equipo de backend en eso?
- ¿Cómo es el día a día en cuanto a code reviews, despliegues y toma de decisiones técnicas?
- ¿Cómo se ve el éxito en este rol en los primeros 3 a 6 meses?
- ¿Cuál es el desafío técnico más grande que enfrenta el equipo hoy?
- ¿Usan arquitectura event-driven en producción o es algo hacia lo que están evolucionando?

---

## Checklist Pre-Entrevista

- [ ] Solicitar a ACTIF que identifique la empresa
- [ ] Investigar la empresa real una vez nombrada
- [ ] Repasar 3 historias STAR
- [ ] Preparar 2-3 preguntas específicas de la empresa
- [ ] Releer la publicación y el CV adaptado
- [ ] Confirmar formato y horario de la entrevista

---

## Post-Entrevista

Enviar un agradecimiento breve a ACTIF dentro de las 24 horas, mencionando un tema concreto de la conversación.

> "Hola [Nombre], gracias por tu tiempo hoy. Disfruté especialmente la conversación sobre [tema], y me entusiasma todavía más la oportunidad. Quedo a disposición por cualquier información adicional. Saludos, Walter"

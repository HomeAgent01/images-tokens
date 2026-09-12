# 🪙 images ($IMAGES) - Advanced ERC-20 Smart Contract

¡Bienvenido al repositorio oficial de **images**, una criptomoneda avanzada basada en el estándar ERC-20 de Ethereum! Este proyecto ha sido diseñado e implementado con un enfoque de arquitectura moderna utilizando **Inteligencia Artificial (Claude)** como copiloto estratégico de desarrollo.

El objetivo principal de este repositorio es demostrar la capacidad de conceptualizar, estructurar, auditar y desplegar un contrato inteligente seguro, optimizando los tiempos de desarrollo mediante técnicas avanzadas de *Prompt Engineering*.

## 🚀 Características del Contrato

A diferencia de un token estándar, **images** incorpora módulos avanzados de seguridad y control de la librería estándar de la industria, **OpenZeppelin**:

*   **Estándar ERC-20:** Implementación nativa de transferencia de valor, saldos y aprobaciones descentralizadas.
*   **Módulo Ownable (Control de Acceso):** Define un propietario único (deployer) con permisos exclusivos para gobernar el contrato.
*   **Módulo Pausable (Mecanismo de Emergencia):** Permite al propietario congelar todas las transferencias de la red de forma inmediata en caso de detectar una vulnerabilidad o exploit.
*   **Módulo Burnable (Deflación):** Permite a los usuarios destruir voluntariamente sus propios tokens para reducir el suministro circulante.
*   **Función Mint Exclusiva:** El propietario puede emitir nuevos tokens de forma controlada según las necesidades del ecosistema.

## 🛠️ Stack Tecnológico y Herramientas

*   **Lenguaje:** Solidity (^0.8.20)
*   **Librerías de Seguridad:** OpenZeppelin Contracts (v5.x)
*   **Entorno de Desarrollo:** Remix IDE
*   **Asistente de IA:** Claude (Anthropic) - Utilizado para la generación de estructuras, auditoría de vulnerabilidades comunes (como Reentrancy) y optimización de gas.

## 💻 Metodología de Desarrollo con IA

Este proyecto se ha desarrollado bajo la metodología de "Desarrollador Asistido por IA". En lugar de realizar una copia ciega de código, se utilizaron prompts iterativos para:
1. Generar la arquitectura base combinando múltiples herencias en Solidity.
2. Adaptar la sintaxis a los cambios de la versión v5 de OpenZeppelin (inicialización explícita del `Ownable(msg.sender)`).
3. Comprender y documentar la necesidad de la función interna `_update` para la resolución de conflictos de herencia entre ERC20 y ERC20Pausable.

---
*Nota: Este proyecto fue desplegado y probado exitosamente de forma gratuita en el entorno simulado Remix VM.*

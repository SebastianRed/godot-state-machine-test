<div align="center">
  <img src="https://img.shields.io/badge/Godot_Engine-4.x-478CBF?style=for-the-badge&logo=godot-engine&logoColor=white" alt="Godot Engine 4.x">
  <img src="https://img.shields.io/badge/GDScript-4.x-478CBF?style=for-the-badge&logo=gdscript&logoColor=white" alt="GDScript 4.x">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License: MIT">
</div>

<h1 align="center">Godot 4: Máquina de Estados Finita (FSM)</h1>

---

<h2>📄 Descripción del Proyecto</h2>

<p>Este proyecto de Godot 4 es un recurso de aprendizaje y una <strong>implementación práctica de una Máquina de Estados Finita (FSM)</strong>. Su objetivo principal es demostrar cómo estructurar, gestionar y aplicar un sistema de estados avanzado y reutilizable para el comportamiento de personajes y otras entidades en tus juegos.</p>

<p>El objetivo principal de este proyecto es:</p>

<ul>
  <li>Crear una <strong>arquitectura de FSM modular y extensible</strong> utilizando nodos de Godot.</li>
  <li>Manejar <strong>transiciones de estado</strong> de manera limpia y organizada.</li>
  <li>Integrar la FSM con un <strong>personaje <code>CharacterBody2D</code></strong>, gestionando su movimiento y estados de forma eficiente.</li>
  <li>Mantener el código <strong>limpio, escalable y fácil de depurar</strong> mediante la separación de preocupaciones.</li>
</ul>

---

<h2>✨ Características Destacadas</h2>

<ul>
  <li><strong>Clase Base de Estado (<code>state.gd</code>):</strong> Hereda de <code>Node</code> para aprovechar las funcionalidades del árbol de escenas (señales, grupos).</li>
  <li><strong>Máquina de Estados Centralizada (<code>state_machine.gd</code>):</strong> Actúa como el controlador principal, delegando la lógica al estado actual y gestionando las transiciones.</li>
  <li><strong>Estados Concretos del Jugador:</strong> Ejemplos claros como <code>player_idle_state.gd</code>, <code>player_walk_state.gd</code>, y <code>player_jump_state.gd</code> demuestran la encapsulación de la lógica.</li>
  <li><strong>Integración con <code>CharacterBody2D</code>:</strong> Muestra la interacción correcta con las propiedades de movimiento de Godot (<code>velocity</code>, <code>is_on_floor()</code>) y el método <code>move_and_slide()</code>.</li>
  <li><strong>Comunicación Segura entre Estados y FSM:</strong> Implementa un método robusto para solicitar cambios de estado, evitando errores comunes de reasignación de métodos.</li>
  <li><strong>Estructura de Carpetas Organizada:</strong> Propone una distribución lógica y escalable de archivos para mantener el proyecto ordenado.</li>
</ul>

---

<h2>📂 Estructura de Carpetas</h2>

<pre><code>res/
├── src/
│   ├── scripts/
│   │   ├── core/
│   │   ├── characters/
│   │   │   ├── player/
│   │   │   │   └── states/
│   │   │   └── enemies/
│   │   └── ui/
│   └── scenes/
│       ├── characters/
│       └── levels/
│
└── assets/
    ├── sprites/
    ├── audio/
    └── fonts/</code></pre>

---

<h2>🤝 Notas</h2>

<p>Este es un proyecto personal de aprendizaje. </p>

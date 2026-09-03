# Cena de fin de año

Página para la Comisión de Eventos Familiar: cualquiera propone un lugar
para la cena de fin de año y el resto vota su favorito, sin registrarse.

**Datos:** todo lo que se ve —propuestas, votos y sus totales— sale en vivo
de Supabase (proyecto `curso-ejemplo02Sept`, tablas `registros` y `votos`).
Nada está escrito a mano en el HTML.

**`.claude/agents/revisor-antes-de-publicar.md`:** un subagente que revisa
la rama antes de publicar (llaves expuestas, cambios de más, errores). Se
invoca pidiéndole a Claude "revisa esto antes de publicar".

**Para continuar:** abre una sesión de Claude sobre este repositorio y pide
el cambio en español. Trabaja en una rama, abre el Pull Request y al
fusionarlo despliega automático a Netlify y a Supabase. Lee `CLAUDE.md`
primero: ahí están las reglas del proyecto.

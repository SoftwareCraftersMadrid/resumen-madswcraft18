# Git branching: No solo git flow
---

Comentamos de pasada distintas estrategias de branching: Una rama por funcionalidad (Branch Per Feature Deployment Strategy), Estrategia basada en entornos (Environment Based Branching Strategy), Estrategia de ramificación basada en lanzamientos (Release Branching Strategy), git flow, Estrategia Mainline Branch, y trunk based. [Más info](https://www.javacodegeeks.com/2015/11/git-branching-strategies.html) o [traducción al español](https://jesuslc.com/2015/12/30/estrategias-de-branching-no-solo-existe-git-flow/)

Hubo mucho dialogo en torno a *trunk based* sobre como implementarlo y que la idea es tener como objetivo commitear en master ya que para llegar a ese punto habremos pulido mucho nuestro proceso de desarrollo: Test rápidos y que cubren todo el código, sistema de CI bien montando, Imágenes de docker por cada push, confianza en el equipo, pairing...

También comentamos que no mola hacer code reviews/pull reuqest a personas sentadas a 2 sillas de distancia. Sería más facil hablarlo con esa persona para poder explicar la intención. O intentar hacer más pairing en vez de code reviews.


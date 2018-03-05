# Effects, co-effects and subscriptions in SPAs (and ClojureScript)

Ponente: [Manuel Rivero](https://twitter/trikitrok)
Slides: [Effects y co-effects](https://drive.google.com/file/d/1VtVziPtOvI68AQiMcq5nq2YGO1YI_x4D/view)

Podríamos definir *side-effect* como aquello que una función hace al *mundo* exterior. De la misma forma,
podríamos definir *side-cause* como aquello que el mundo hace a mi función (datos que necesita mi función
pero no es pasado como parámetro).

Así, un *effect* sería un *side-effect* y un *co-effect* sería un *side-cause*.

Para conseguir que mis funciones no dependan del mundo exterior, se podría aplicar un concepto que se parece mucho a
inyección de dependencias, pero aplicado a funciones. La idea es que ahora, mis funciones reciben co-effects y devuelven
effects. Del manejo de effects y co-effects se encarga el lenguaje o la librería en cuestión, dejando a tus funciones como
funciones puras, fácilmente entendibles, fácilmente testeables.

Subscripciones de la librería [re-frame](https://github.com/Day8/re-frame) (librería ClojureScript con un concepto similar
a React en JavaScript): funciones que hacen una query sobre el estado de la applicación y el resultado lo pasan
a las funciones que renderizan la vista.
Similar a las funciones de [ReactiveX](/blog/2017/12/12/programacion-reactiva-javascript/) que proporciona funciones que
puedes ir encadenando.

Manuel recomendó una charla,  [Unidirectional data flow architectures](https://vimeo.com/168652278). Ha costado un poco dar con ella, pero por el camino, apareció un artículo que parece estar bastante relacionado: [Unidirectional user interface architectures](https://staltz.com/unidirectional-user-interface-architectures.html), tanto la charla como el artículo son de André Staltz.

## [:coffee: Buy me a coffee](https://www.buymeacoffee.com/risto1)

```prolog
name('Risto Stevcev').
email('risto1@gmail.com').
email('me@risto.codes').
website('https://risto.codes').
support('Buy me a coffee', 'https://www.buymeacoffee.com/risto1').

research(lisp, (conditions, restarts)).

research(common_lisp, X) :-
    research(lisp, X).

research(prolog, dcgs).
research(prolog, chrg).
research(prolog, clp).

research(swi, X) :-
    research(prolog, X).

research(tau, X) :-
    research(prolog, X).

grammar(prolog, dcgs).
grammar(prolog, chrg).

grammar(X) :-
    grammar(_, X).

peg(dcgs, tabling).

effects(lisp(conditions)).
coroutines(js(generators)).
coroutines(lisp(conditions)).

monotonic(prolog).

resource(prolog, 'https://www.metalevel.at/prolog').
resource(prolog, 'https://www.swi-prolog.org').

resource(logic, X) :-
    resource(prolog, X) ;
    resource(datalog, X) ;
    resource(rdf, X) ;
    resource(turtle, X) ;
    resource(owl, X).
```

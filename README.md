# Le Pomme Es Ne Jete
A procedural dialogue generator for use outside of story specific events. The eventual direction I want to go is "Bamboo Francais", for my science fiction and fantasy setting.

## Demo
<iframe width="560" height="315" src="https://www.youtube.com/embed/D4z92kMQkAw?si=Oe6Y4kHHimyhoS6o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Generation of Francais
~~~
la orange orange es mange.   The orange orange is eaten. 
le pomme rouge es ne jete.   The apple red is tossed out. 
le pomme rouge es mange.     The apple red is eaten. 
le pomme rouge es ne jete.   The apple red is tossed out. 
les banane jaune es ne jete. The banana yellow is not tossed out 
le pomme rouge es mange.     The apple red is eaten. 
le pomme rouge es mange.     The apple red is eaten. 
les banane jaune es ne jete. The banana yellow is not tossed out 
la orange orange es ne jete. The orange orange is tossed out. 
le pomme rouge es mange.     The apple red is eaten. 
le pomme rouge es mange.     The apple red is eaten. 
les banane jaune es ne jete. The banana yellow is not tossed out 
le pomme rouge es mange.     The apple red is eaten. 
les banane jaune es ne jete. The banana yellow is not tossed out 
la orange orange es ne jete. The orange orange is tossed out. 
la orange orange es ne jete. The orange orange is tossed out. 
les banane jaune es ne jete. The banana yellow is not tossed out 
la orange orange es mange.   The orange orange is eaten. 
les banane jaune es mange.   The banana yellow is eaten. 
la orange orange es ne jete. The orange orange is tossed out. 
le pomme rouge es mange.     The apple red is eaten. 
le pomme rouge es mange.     The apple red is eaten. 
le pomme rouge es ne jete.   The apple red is tossed out. 
le pomme rouge es mange.     The apple red is eaten. 
les banane jaune es ne jete. The banana yellow is not tossed out 
les banane jaune es ne jete. The banana yellow is not tossed out 
la orange orange es mange.   The orange orange is eaten. 
le pomme rouge es ne jete.   The apple red is tossed out. 
le pomme rouge es mange.     The apple red is eaten. 
~~~

## Statistics from Francais
~~~
la orange orange es mange. [:correct, 0.07142857142857142] 
le pomme rouge es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
le pomme rouge es ne jete. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
la orange orange es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
la orange orange es ne jete. [:correct, 0.07142857142857142] 
la orange orange es ne jete. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
la orange orange es mange. [:correct, 0.07142857142857142] 
les banane jaune es mange. [:correct, 0.07142857142857142] 
la orange orange es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
le pomme rouge es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
les banane jaune es ne jete. [:correct, 0.07142857142857142] 
la orange orange es mange. [:correct, 0.07142857142857142] 
le pomme rouge es ne jete. [:correct, 0.07142857142857142] 
le pomme rouge es mange. [:correct, 0.07142857142857142] 
~~~


## Next Generation
~~~
fruits.train(:contrastive, "Le pomme rouge es jete, mais le banana jaune es ne jete pas.",  "contrastive")
fruits.train(:contrastive, "Le banane jaune es jete, mais le pomme rouge es ne jete pas.",  "contrastive")
fruits.train(:contrastive, "L'orange orange es jete, mais le banana jaune es ne jete pas.", "contrastive")
fruits.train(:contrastive, "Le banane jaune es jete, mais l'orange es ne jete pas.",        "contrastive")
~~~

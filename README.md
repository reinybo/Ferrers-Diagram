# Ferrer's Diagrams for Manim
Manim implementation of Ferrer's/Young diagrams, a tool for visualizing partitions and partition bijections.
```
class FerrersDiagramDemonstration(Scene):
    def construct(self):
        ferrers_diagram = FerrersDiagram(partition_sequence=np.array([3,7,9,5,7]))
        self.play(ShowCreation(ferrers_diagram))
        self.play(SortingParts(ferrers_diagram))
        self.play(FranklinInvoluting(ferrers_diagram))
        self.play(Conjugating(ferrers_diagram))
        self.play(Convoluting(ferrers_diagram))
```
![](Demo.gif)

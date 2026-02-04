# TeAAL specifications on variants of Loops' SpMV implementations

Variants:
- Original
- Thread-Mapped
- Group-Mapped
- Work-Oriented
- Merge Path

Loops github repo: https://github.com/gunrock/loops

Terminology (From Muhammad Osama's Dissertation: [Load Balancing on the GPU](https://arxiv.org/abs/2212.08964)):
- Work item/atom: A single unit of work that is to be scheduled onto the GPU. We assume that all work atoms have an equal cost during execution.
- Work tile: A collection of work items. Work tiles may have different costs during execution.
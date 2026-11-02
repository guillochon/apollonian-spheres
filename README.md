# Apollonian Sphere Generations: OEIS A154639–A154645

**https://guillochon.github.io/apollonian-spheres/**

Start with three unit balls between two parallel plates, five objects that all touch. Any four of them leave room
for exactly one more ball touching all four, so the gaps can be filled forever: the three-dimensional Apollonian
packing. Colin Mallows (J. Integer Sequences, 2009) counted the balls added in each generation, and the sums of
their curvatures, in two ways ("strategy (a)" and "strategy (b)"). These are OEIS A154639–A154645.

The page draws the packing as polished-metal spheres, colored by generation:

- **Generations 0–12.** Every sphere through generation 8 (117,448), and every sphere of radius at least 1/150 in
  generations 9–12, 1.21 million in all; smaller ones are under a pixel at these distances. Generations 9–12 load
  when the slider reaches them (about 23 MB).
- **Both strategies,** and a mode that highlights the spheres strategy (b) counts earlier than strategy (a).
- **Cutaway, newest-generation-only and a grow animation;** hover a sphere for its bend and both generations.
- **The seven sequences,** with Mallows's terms checked: six of them corrected, all extended, and generating
  functions for A154639–A154642.

Each sphere is ray-traced on a camera-facing quad in a fragment shader (three.js), reflecting a studio
environment rendered once into a cube map.

The proofs, the independent checks and the programs that produced every sphere and term are in
[oeis-results/A154640](https://github.com/guillochon/oeis-results/tree/main/A154640).

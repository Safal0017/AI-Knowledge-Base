# Trigonometry: Sin, Cos, Tan

**Video:** [sin cos tan explained. Explanation using real life example | Math, Statistics for data science](https://www.youtube.com/watch?v=o6nFv0UfEdI)

**Playlist:** [Mathematics, statistics for data science and machine learning](https://www.youtube.com/playlist?list=PLeo1K3hjS3uuKaU2nBDwr6zrSOTzNCs0l)

This note covers sine, cosine, and tangent using the two real-life examples from the video: measuring a tree height and resolving force into horizontal and vertical components. The goal is intuition first, then formulas, then ML relevance.

## What Problem Are We Solving?

Trigonometry helps us find unknown lengths or force components when we know an angle and one side of a right triangle.

That is useful in engineering, physics, and also in machine learning later through concepts like cosine similarity.

## Core Intuition

A right triangle has one 90-degree angle. Once you know one acute angle, the side ratios become predictable.

The key idea is not memorizing random formulas. It is understanding that angles and side ratios have a stable relationship.

| Function | Uses |
|---|---|
| Tan | Relates opposite side to adjacent side |
| Sin | Relates opposite side to hypotenuse |
| Cos | Relates adjacent side to hypotenuse |

## Tree Height Example

The video starts with a forest officer who wants to measure the height of a tree without climbing it.

Known values:

- Distance from tree = 50 feet
- Angle to the top of the tree = 30 degrees

This forms a right triangle.

### Triangle view

```text
        top of tree
            /|
           / |
          /  |
         /   |  height = x
        /30° |
       /_____| 
      50 ft
```

### Tan formula

Formula:

```text
tan(theta) = opposite side / adjacent side
```

For this tree example:

```text
tan(30°) = x / 50
```

From the video, `tan(30°) = 0.577`.

So:

```text
0.577 = x / 50
x = 50 * 0.577
x = 28.85 feet
```

That means the tree height is approximately 28.85 feet.

## Why Tan Works Here

Tangent is useful when you know:

- an angle,
- the horizontal distance,
- and you want the vertical height.

This makes tan a natural fit for height estimation, slope calculation, and many geometry problems.

## Tan Reference Table

| Angle | tan(angle) |
|---|---:|
| 0° | 0 |
| 1° | 0.0174 |
| 2° | 0.0349 |
| 30° | 0.577 |
| 45° | 1 |

The video emphasizes that these are fixed relationships for a given angle.

## Pythagoras Connection

Before explaining sine and cosine, the video uses Pythagoras theorem.

Formula:

```text
hypotenuse^2 = base^2 + height^2
```

If a triangle has sides 3 and 4, then the hypotenuse is 5.

This becomes important because sine and cosine use the hypotenuse.

## Force Component Example

The second example is a package being pulled with a rope.

Known values:

- Total force = 10 newton
- Rope angle = 30 degrees

The force can be split into two parts:

- Horizontal component `X_f`
- Vertical component `Y_f`

| Component | Meaning |
|---|---|
| `X_f` | Helps pull the package horizontally |
| `Y_f` | Helps lift the package upward |

## Why Split Force?

If the rope is pulled at an angle, the total force is not acting in one direction only. Part of it moves the object forward, and part of it lifts it slightly.

This is a very common physics idea and also a good way to understand trigonometric projection.

## Sin Formula

Formula:

```text
sin(theta) = opposite / hypotenuse
```

For the package example:

```text
sin(30°) = Y_f / 10
```

From the video, `sin(30°) = 0.5`.

So:

```text
0.5 = Y_f / 10
Y_f = 5 newton
```

The vertical force component is 5 newton.

## Cos Formula

Formula:

```text
cos(theta) = adjacent / hypotenuse
```

For the package example:

```text
cos(30°) = X_f / 10
```

From the video, `cos(30°) = 0.866`.

So:

```text
0.866 = X_f / 10
X_f = 8.66 newton
```

The horizontal force component is 8.66 newton.

## Sin And Cos Table

| Angle | sin(angle) | cos(angle) |
|---|---:|---:|
| 0° | 0 | 1 |
| 30° | 0.5 | 0.866 |
| 45° | 0.707 | 0.707 |
| 90° | 1 | 0 |

This table helps build intuition that as angle increases, sine rises and cosine falls.

## Simple Memory Trick

| Function | What it focuses on |
|---|---|
| Tan | Opposite / Adjacent |
| Sin | Opposite / Hypotenuse |
| Cos | Adjacent / Hypotenuse |

A practical way to remember them:

- Tan uses the two shorter sides.
- Sin and cos use the longest side.

## Real-Life Meaning

| Concept | Real-life meaning |
|---|---|
| Tan | Finding height from distance and angle |
| Sin | Finding vertical contribution of a tilted force |
| Cos | Finding horizontal contribution of a tilted force |

This is why these concepts are not just school math. They solve real measurement problems.

## Data Science Relevance

The video connects trigonometry to data science through future cosine similarity.

Cosine similarity is used to compare vectors, especially in NLP, embeddings, and recommendation systems.

That means the trigonometry here is not isolated theory. It becomes useful later when comparing directions rather than raw magnitudes.

## Deep Learning Relevance

Trigonometry shows up indirectly in deep learning through:

- cosine similarity for embeddings,
- vector comparisons,
- attention-related geometric intuition,
- representation learning.

You do not use sine and cosine every day in model code, but you do use the geometric ideas behind them.

## Systems Engineering Relevance

In ML systems, vector similarity matters a lot.

Examples:

- semantic search,
- embedding retrieval,
- recommendation engines,
- nearest-neighbor lookup,
- duplicate detection.

Cosine similarity is a practical systems-level use of this topic.

## Common Mistakes

- Mixing up opposite and adjacent sides.
- Forgetting that the hypotenuse is the longest side.
- Using the wrong trigonometric function.
- Treating angle and side values as interchangeable.
- Memorizing formulas without understanding triangle layout.

## Key Takeaways

- Trigonometry helps relate angles and side lengths in right triangles.
- Tan is opposite over adjacent.
- Sin is opposite over hypotenuse.
- Cos is adjacent over hypotenuse.
- Tan helps with height estimation.
- Sin and cos help split force into components.
- This foundation later supports cosine similarity in machine learning.

## Revision Cheat Sheet

- **Tan** = opposite / adjacent
- **Sin** = opposite / hypotenuse
- **Cos** = adjacent / hypotenuse
- **30°** is a common reference angle in examples
- **Pythagoras** helps relate triangle sides
- Trigonometry is useful for geometry, force, and vector similarity

## 30-Second Revision

Trigonometry studies the relationship between angles and sides of a right triangle. Tan is opposite over adjacent, sin is opposite over hypotenuse, and cos is adjacent over hypotenuse. In the video, tan is used to find tree height, and sin/cos are used to split a 10 newton force into vertical and horizontal parts.

## 2-Minute Revision

If you know one angle in a right triangle, trig functions let you calculate missing sides. In the tree example, tan(30°) gives the ratio between tree height and distance from the tree. In the package example, sine gives the vertical force component and cosine gives the horizontal force component. These relationships are fixed for a given angle and are very useful in real-world measurements.

## Interview Perspective

Common interview question: what is the difference between sin, cos, and tan?

A strong answer:

- Tan relates opposite and adjacent sides.
- Sin relates opposite and hypotenuse.
- Cos relates adjacent and hypotenuse.

Another common question: why is trigonometry relevant to machine learning?

Because cosine-based geometry is used in vector similarity and embedding comparisons.

## Engineering Perspective

In real systems, geometric thinking shows up in vision, robotics, signal processing, and vector search. In ML systems, the biggest practical connection is cosine similarity and direction-based comparison of embeddings.

## Next Topic Recommendation

The next topic should be cosine similarity, because this video was clearly setting that up as the bridge from trigonometry to ML.

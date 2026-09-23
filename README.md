_This project has been created as part of the 42 curriculum by tmkrtumy._

# fract-ol

## Description

The **main goal** of fract-ol is to discover **fractal geometry** and learn how mathematical formulas can be transformed into something visual.

In this project, we generate and render different fractals using **MiniLibX**:

* **Mandelbrot set**
* **Julia set**
* **Burning Ship fractal**

Besides simply drawing them, we can **zoom**, **move around**, **change colors**, increase the rendering quality, and modify the Julia set in real time.

The project is also a good introduction to working with **complex numbers**, coordinate transformations, graphical rendering, and event handling.

One of the interesting things about fractals is that relatively simple formulas can generate incredibly complicated patterns. By continuously applying the same formula to every pixel, we can decide whether a point belongs to the fractal and assign it a color depending on how quickly it escapes.

## Instructions

### Compilation

Compile the project with:

```bash
make
```

The project also provides shortcuts for compiling and immediately launching each fractal:

```bash
make m
```

Launches the **Mandelbrot set**.

```bash
make j
```

Launches the **Julia set**.

```bash
make s
```

Launches the **Burning Ship fractal**.

There are also equivalent Valgrind commands:

```bash
make vm
make vj
make vs
```

### Execution

The program can also be executed manually.

Mandelbrot:

```bash
./fractol mandelbrot
```

Julia:

```bash
./fractol julia <real> <imaginary>
```

For example:

```bash
./fractol julia -0.8 0.156
```

Burning Ship:

```bash
./fractol burning_ship
```

If the arguments are invalid, the program prints the available options.

### Controls

| Key       | Action                            |
| --------- | --------------------------------- |
| `+`       | Zoom in                           |
| `-`       | Zoom out                          |
| `W` / `↑` | Move up                           |
| `A` / `←` | Move left                         |
| `S` / `↓` | Move down                         |
| `D` / `→` | Move right                        |
| `Space`   | Change color and increase quality |
| `J`       | Rotate / modify the Julia set     |
| `Esc`     | Exit                              |

The fractals can therefore be explored interactively instead of being rendered as a single static image.

## Resources

The following resources were useful for understanding the concepts used in this project:

* [Mandelbrot set — Wikipedia](https://en.wikipedia.org/wiki/Mandelbrot_set)
* [Julia set — Wikipedia](https://en.wikipedia.org/wiki/Julia_set)
* [Burning Ship fractal — Wikipedia](https://en.wikipedia.org/wiki/Burning_Ship_fractal)
* [Complex number — Wikipedia](https://en.wikipedia.org/wiki/Complex_number)
* MiniLibX documentation and examples
* X11 keyboard event documentation

### AI usage

AI was used as an additional learning and debugging tool during the project.

In particular, it was used for:

* explaining some of the mathematics behind fractals and complex numbers;
* discussing coordinate scaling between the screen and the complex plane;
* debugging and reviewing parts of the implementation;
* improving documentation and the README.

The fractal algorithms, rendering logic, event handling, and final implementation were written and tested as part of the project.


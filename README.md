# GTK4_Tutorial
>Resources available at [ ToshioCP /Gtk4-tutorial](https://github.com/ToshioCP/Gtk4-tutorial)

## How to build files?

### Via shell script
- Type the following command:

``` sh
sh ./build.sh {name-of-file}
```
- Execute the file:

```sh
./{name-of-file}
```

### Via CMake
- Create `build` directory:
```sh
mkdir build/
```

- Change directory to build:

```sh
cd build
```
- Generate files using `cmake`:

```sh
cmake ..
```

- Build using `cmake`:

```sh
cmake --build .
```

- Execute the file

```sh
./{name-of-file}
```


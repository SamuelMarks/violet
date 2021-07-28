# Violet - Lightweight STUN/TURN server

Violet is a lightweight STUN/TURN server ([RFC8489](https://tools.ietf.org/html/rfc8489) and [RFC8656](https://tools.ietf.org/html/rfc8656)) written in C without dependencies, based on [libjuice](https://github.com/paullouisageneau/libjuice).

![Oompa-Loompas rolling Violet, from Charlie and the Chocolate Factory](https://github.com/paullouisageneau/violet/blob/master/image.png?raw=true)

> "Mercy! Save us!" yelled Mrs Beauregarde. "[...] Violet, you’re **turn**ing violet, Violet!" [...]
>
> "Squeeze her," said Mr Wonka. "We've got to squeeze the **juice** out of her immediately."
>
> -- Charlie and the Chocolate Factory, Roald Dahl

## Dependencies

None!

## Building

### Clone repository and submodules

```bash
$ git clone https://github.com/paullouisageneau/violet.git
$ cd violet
$ git submodule update --init --recursive
```

### Build with CMake

```bash
$ cmake -B build
$ cd build
$ cmake --build .
```

## Running

Running the TURN server with default options is as simple as:
```bash
$ ./violet --credentials USER:PASSWORD
```

Available options can be listed with the `--help` (or `-h`) flag:
```bash
$ ./violet --help
```

## Links

Violet is available as a [package on AUR](https://aur.archlinux.org/packages/violet/).


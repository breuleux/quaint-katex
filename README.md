
# quaint-katex

Katex support for Quaint

## Install

In your Quaint project directory, run the command:

    quaint --setup katex


## Usage

The plugin defines two operators:

* `$+[...]` inserts math inline
* `$$ ...` displays one or more equations

For example:

```
Inline math! $+[x_1 + x_2]

Display math!

$$ \sum_{i=1}^{1000} x_i + y_i^2 + z_i^3

```

Instead of LaTeX's awkward line break syntax, you can use bullet
points in the environment created by `$$` to list multiple equations,
for example:

```
$$
  * x & = y + z
  * x - y & = z
```


### Wrap with a class

Instead of an environment, or in addition to it, you may specify class
descriptions and an id for an equations block:

```
.my-class#some-id $$
  * x & = y + z
  * x - y & = z
```

The above will wrap the equation with `<div class="my-class" id="some-id">...</div>`,
which means you can easily customize the display of various equations.


## Options

There are no options at the moment.


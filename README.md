# brain-turtle

A [brain][brain] library for generating turtle graphics commands that could
potentially be interpreted to draw awesome turtle based graphics!

**NOTE:** This is **not** a working example of anything yet. This library is being
developed so that future versions of the language will be able to use it. This
gives us an idea of what a full library in brain would look like.

## Example

```brain
use package turtle;

for _ in 0..3 {
  turtle::forward(100);
  turtle::turn(120);
}
```

## Future Enhancements

These are enhancements that could happen very soon, but we are just not sure
how yet.

- [ ] Getting values for turtle properties (pen::is_down(), etc.)
    - This is a hard problem because we don't keep any state so we would have to
      query with an output command and then read/parse input. Parsing is hard
      because we don't have a very sophisticated IO model. Maybe with a good,
      buffered IO library we could support parsing. This means that we would
      have to wait for the allocator to get implemented.
- [ ] Unit tests
    - This will require a unit testing framework to be built.

## Far Future Enhancements

- [ ] Floating point arguments

[brain]: https://github.com/brain-lang/brain

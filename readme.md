# stencil-inert-missing-from-types

This shows that Stencil's types do not include the `inert` attribute, which is [now supported by all major browsers]()https://caniuse.com/?search=inert.

## Steps to reproduce

1. Clone this repo
2. `npm install`
3. `npm run build`

This will produce the following error:

```cli
Type '{ inert: true; }' is not assignable to type 'HTMLAttributes<HTMLDivElement>'.Property 'inert' does not
     exist on type 'HTMLAttributes<HTMLDivElement>'.
```
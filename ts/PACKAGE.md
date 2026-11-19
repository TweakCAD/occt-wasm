# @tweakcad/occt-wasm

TweakCAD's build of [occt-wasm](https://github.com/andymai/occt-wasm), made from
the `tweakcad` branch of [TweakCAD/occt-wasm](https://github.com/TweakCAD/occt-wasm).
Version `<upstream>-tweakcad.<n>` is upstream release `<upstream>` plus the commits
on that branch; the API is upstream's. To keep `import ... from 'occt-wasm'`:

```bash
npm install occt-wasm@npm:@tweakcad/occt-wasm
```

Patches in this version, on top of upstream:

- `unifySameDomainWithin`: a same-domain merge within given linear and angular
  tolerances.
- Every `*WithHistory` result also names sub-shapes by input, kind and position
  (the `*Indexed` lists), beside the hash lists.
- Heap addresses cross to JavaScript unsigned, so the heap can grow past 2 GB.

The rest of this file is upstream's README.

---


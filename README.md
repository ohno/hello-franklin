## 1. hello-franklin

1. Install [Franklin.jl](https://github.com/JuliaDocs/Franklin.jl).
```julia
import Pkg; Pkg.add("Franklin")
```

2. Generate newsite and start the server.
```julia
using Franklin
newsite("hello-franklin")
serve()
```

3. Fix Julia version (<=1.11) in Deploy.yml.

https://github.com/ohno/hello-franklin/blob/a24ee503a80ef92f72cc0470d728c7f7200c2963/.github/workflows/Deploy.yml#L28

4. Change settings in https://github.com/ohno/hello-franklin/settings/pages for GitHub Pages.
    - Source: Deploy from a branch
    - Branch: gh-pages/(root)

5. Visit https://ohno.github.io/hello-franklin/.

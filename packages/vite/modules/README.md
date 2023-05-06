# Do not Touch deps your self
it is also excluded from via .gitignore 
when you want to patch or modify the content in deps you need to create a new file and import the code from deps then
you modify the exported objects as you need and re export them then you bundle up and your done.

This concept is importent as we do not plan to contribute back to that legacy deps like the vite hmr loader or typescripts
typescript compiler only the typechecker is usefull 

## usage
Showing the bundler interface
```
<script type="module" src="node_modules/vite/modules/vite.js"></script>
<vite-bundler></vite-bundler>
```

showing the bundler result returns a iframe with the vite result like stackblitz does 
```
<script type="module" src="node_modules/vite/modules/vite.js"></script>
<vite-bundle src="vite.config.js"></vite-bundle>
```

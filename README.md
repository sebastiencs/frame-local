# Frame local
[![MELPA](http://melpa.org/packages/frame-local-badge.svg)](http://melpa.org/#/frame-local)

Access variables local to a frame  

You can use the functions frame-local-[set,get,setq,getq]  
With frame-local-[setq,getq], the variables must not be quoted.  

It is recommended to prefix the variables with your package name  
to not create conflicts with variables from other packages.  

Examples:
```el
(frame-local-set 'my-variable 1)
(frame-local-get 'my-variable)
(frame-local-setq my-other-variable 2 some-frame)
(frame-local-getq my-other-variable some-frame)
```

Note that the variables created with this package don't have any  
relation with variables defined by `defvar`, `defconst` etc.  

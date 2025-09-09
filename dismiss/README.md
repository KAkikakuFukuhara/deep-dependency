# README

これは失敗例。  

以下がエラー。  
```console
Because subb (0.1.0) depends on subc (0.1.0) @ deep-dependency/dismiss/pkgs/subb/pkgs/subc and suba (0.1.0)  depends on subc (0.1.0) @ deep-dependency/dismiss/pkgs/suba/pkgs/subc, subb (0.1.0)is incompatible with suba (0.1.0). 
So, because dismiss depends on both suba (0.1.0) and subb (0.1.0) , version solving failed.
```
  何が言いたいのかというと、subcという同一名パッケージがsuba, subbで異なる場所から参照されていることにより、subaとsubbをインストールできないというエラーである。  

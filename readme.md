# Práctica GIT

### Murgui Gómez, Núria

--

**1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset --hard HEAD~1` 

Porque con el reset hard se deshacen el commit y los cambios que se hayan realizado. Si no hubiese utilizado el --hard los cambios no hubiesen desaparecido. 

--

**2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog y git reset --hard 155fb2b  ` 

El primer comando lo utilizcé para acceder al identificador del commit que acababa de borrar y así poder volver a este paso con el segundo comando. 

--

**3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No causó ningún conflicto porque no se habían producido cambios en un mismo documento a la misma altura. La rama que estamos intentando unir (merge), es padre del commit de la rama en la que ya estoy (styled) por tanto los comits se guarda como uno sucesivo de otro y no genera conflicto.

--

**4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

En este caso sí causó un conflicto porque se han producido cambios en un mismo documento en ramas distintas a la misma altura.

--

**5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No causó ningún conflicto porque no se ha producido ningún cambio. Al producirse el conflicto anterior se han dejado los cambios de la rama styled que ya había cuando styled ha hecho el merge con master. Por tanto ahora master puede hacer un merge con styles sin problemas. 

--

**6. ¿Qué comando o comandos utilizaste en el paso 25?**

`git graph ` 

--

**7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí que podría serlo, de hecho lo hubiese sido si no hubiésemos especificado el comando `git merge --no-ff title` para que fuese no fast-forward..  Esto se debe a que el commit de la rama title es un descendiente directo de la rama master, lo que produciría un merge fast-forward.

--


**8. ¿Qué comando o comandos utilizaste en el paso 27?**

`git reset HEAD~1 ` 

--

**9. ¿Qué comando o comandos utilizaste en el paso 28?**

`git checkoout -- don-quijote.md` 

--

**10. ¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -d title` y `git branch -D title` 

--

**11. ¿Qué comando o comandos utilizaste en el paso 30?**

`git  reflog`  y  `git reset --hard 9ef6531` También podría haberse utilizado `git checkoout 9ef6531`, con lo que posteriormente deberíamos haber vuelto a la rama master con `git checkoout master`.
` 
--

**12. ¿Qué comando o comandos usaste en el paso 32? **

`git reflog` y `git reset --hard 73706ba` 

--

**13. ¿Qué comando o comandos usaste en el punto 33?**

`git reflog` y `git reset --hard 4836ff9
` 
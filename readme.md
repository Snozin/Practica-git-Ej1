# Práctica del curso de Git

## Ejercicio 1

**¿Qué comando utilizaste en el paso 11? ¿Por qué?**
> Utilicé `git reset --hard HEAD~1` porque permite mover el puntero sobre el que esté situado *HEAD* hacia el commit inmediatamente anterior sin guardar los cambios del working area.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
> Utilicé `git reset --hard <hash>` porque así podía revertir al identificador del commit que necesitaba en este caso y recuperar además el contenido del working area en el proceso.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
> No, porque la rama *styled* ya contenía todos los cambios que se habían hecho previamente sobre la rama *main* y en este caso el merge fue *fast-forward*.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
> Sí, porque había varios cambios que afectaban a las mismas partes del código de ambas ramas y por esto hubo que seleccionar los cambios que queríamos preservar y el merge no pudo ser *fast-forward*.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
> No, tampoco hubo conflictos. En este caso el merge se produgo *fast-forward* sin inconvenientes.

**¿Qué comando o comandos utilizaste en el paso 25?**
> Usé la variante del log que vimos en clase: `git log --graph` para poder ver una representación del grafo por consola.

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
> Si, podría ser perfectamente *fast-forward* porque la rama *main* contiene todo el trabajo de la rama *title* y unicamente se añade una pequeña modificación al texto.

**¿Qué comando o comandos utilizaste en el paso 27?**
> En este caso volví a usar un `git reset HEAD~1` para desplazarme al estado anterior al merge pero preservando los cambios en el working area.

**¿Qué comando o comandos utilizaste en el paso 28?**
> Aquí utilicé `git restore git-nuestro.md` para eliminar el archivo modificado del working area.

**¿Qué comando o comandos utilizaste en el paso 29?**
> `git branch -D title`

**¿Qué comando o comandos utilizaste en el paso 30?**
> `git reset --hard <hash>`

**¿Qué comando o comandos usaste en el paso 32?**
> Primero `git reflog` para localizar el *hash* y luego `git reset <hash>` para desplazarme hasta el commit inicial.

**¿Qué comando o comandos usaste en el punto 33?**
> `git checkout main` para desplazar el puntero *HEAD* a la rama *main* en su estado final y con los cambios que tuviese en el working area.
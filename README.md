# Soluciones de Exercism

Soluciones de los ejercicios de [exercism](https://exercism.org/)

## Usar exercism

### Instalar

Instruccione para instalar exercism en Windows y Linux

#### Windows

Descargar y ejecutar el [instalador](https://github.com/exercism/windows-installer/releases/latest)

#### Linux

Descargar el archivo [comprimido](https://github.com/exercism/cli/releases/latest) y lo extraemos:

```bash
tar -xf exercism-linux-64bit.tgz
```

Ejecutamos los siguientes comandos:

```bash
mkdir -p ~/bin
```
```bash
mv exercism ~/bin
```

Verificamos de que funcione:

```bash
~/bin/exercism
```

Agregamos al PATH. Para verificar si bin ya esta en el PATH ejecutamos el siguiente comando:

```bash
[[ ":$PATH:" == *":$HOME/bin:"* || ":$PATH:" == *":~/bin:"* ]] && echo "~/bin is in PATH" || echo "~/bin is not in PATH"
```

Si no esta en el PATH lo agregamos con el siguiente comando:

```bash
echo 'export PATH=~/bin:$PATH' >> ~/.bash_profile
source ~/.bash_profile
```

Verificamos de que funcione:

```bash
exercism
```

### Configurar exercism

Para configurarlo agregamos el token a la configuracion usando el comando:

```bash
exercism configure --token={your-token}
```


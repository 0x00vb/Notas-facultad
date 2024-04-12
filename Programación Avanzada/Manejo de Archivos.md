```java
import java.util.*; 
import java.io.*;

public class MuestraContenidoArchivo{
	public static void main(String[] args) throws IOException {
		// 
		File archivoEntrada = new File("archivo.txt");
		while (archivoEntrada.hasNext()){ 
			String linearchivoEntrada = scanner.nextLine();
		}

		//Para asegurar el cierre de los archivos, utilizar siempre finally
		


	}
}

```




## Acceso directo
```java
RandomAccessFile ra = new RandomAccessClass("archivo.txt", "r2");
```

metodos Lectura: readXX()
metodos Escritura: writeXX()

metodos de desplazamiento:
```java
	.getFilePointer() //posicion actual
	.seek(long pos) // Accede a la posicion indicada indicada en bytes
	.length(): //tamaño del archivo	
```


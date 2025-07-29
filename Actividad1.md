# Actividad 1: Representación de Datos en el Mundo Digital
Se solicitó dar el valor de las unidades mostradas en clase a las que equivalían 3 archivos:
## 3 archivos:
- txt 52383 caracteres 
- 5433 datos punto flotante : 5433 × 4=21,732 bytes
- 3434 datos enteros : 3434×4=13,736 bytes

# SOLUCIÓN:
- .txt → 52,383 bytes
- punto flotante → 21,732 bytes
- enteros → 13,736 bytes

52,383 + 21,732 + 13,736= 87,851 bytes
En KB: 87,851 ÷ 1024 ≈ 85.83 KB
​
# SOLUCIÓN PREGUNTAS FINAL DE PÁGINA
## 1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.
R/ Las computadoras están hechas de componentes electrónicos que tienen dos estados estables: encendido (1) y apagado (0). Estos dos estados se representan como bits, y es la forma más sencilla, fiable y eficiente para que los circuitos electrónicos procesen información. Representar los datos en binario permite: Simplificar el diseño del hardware, evitar errores eléctricos causados por múltiples niveles de voltaje, estandarizar el almacenamiento y la transmisión de datos digitales

## 2. Convierte el número binario 10011011 a decimal y a hexadecimal.
R/ a decimal: 128 + 0 + 0 + 16+ 8 + 0 + 2 + 1 = 155
​   a hexadecimal: 1001=9 1011=B; 0X9B

## 3.  Escribe un programa en Python que permita al usuario ingresar un texto y muestre su representación en binario, hexadecimal y ASCII.
R/ def representar_texto():
    texto = input("Ingresa un texto: ")

    print("\nRepresentaciones:")
    for char in texto:
        ascii_val = ord(char)
        binario = format(ascii_val, '08b')
        hexadecimal = format(ascii_val, '02x')
        print(f"'{char}' → ASCII: {ascii_val}, Binario: {binario}, Hex: {hexadecimal}")

representar_texto()

## 4. Investiga y describe cómo se representa una imagen en formato PNG en el disco.
R/ Una imagen PNG se representa en disco como un archivo comprimido estructurado en bloques o chunks. Algunos puntos clave:

- Cabecera (Header): Contiene información como tamaño, profundidad de color, etc.
- Datos comprimidos: Usa el algoritmo DEFLATE, que combina LZ77 y Huffman coding.
- Formato binario: Todo el archivo está codificado en binario, incluyendo colores representados generalmente como valores RGB (Red, Green, Blue).
- Soporta transparencia (canal alfa).

Los datos de la imagen se organizan en píxeles, donde cada píxel tiene componentes de color codificados numéricamente.

## 5. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?
R/ Un byte puede representar números del 0 al 255 Si intentas guardar un número como 300, simplemente no cabe en un solo byte.

- Python no tiene ese límite para enteros, ya que maneja los números de forma dinámica. Por ejemplo:
x = 300
print(x.to_bytes(2, 'big'))  # Correcto: usa 2 bytes para representarlo

- Pero si intentas hacer esto con solo 1 byte te da este error: 
x = 300
print(x.to_bytes(1, 'big'))  # Error: OverflowError

Conclusión: Python evita errores silenciosos y te avisa cuando necesitas más espacio de almacenamiento para representar un número.


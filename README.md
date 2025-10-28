# triangulo
def forma_triangulo(a, b, c):
    return (a < b + c) and (b < a + c) and (c < a + b)


def area_triangulo(a, b, c):
    p = (a + b + c) / 2
    area = (p * (p - a) * (p - b) * (p - c)) ** 0.5
    return area


a = int(input("Digite o numero a: "))
b = int(input("Digite o numero b: "))
c = int(input("Digite o numero c: "))

if forma_triangulo(a, b, c):
    print("Os numeros formam um triângulo.")
    print(f"A área do triângulo é: {area_triangulo(a, b, c):.2f}")
else:
    print("Os numeros não formam um triângulo.")
    print(f"Valores lidos: a = {a}, b = {b}, c = {c}")

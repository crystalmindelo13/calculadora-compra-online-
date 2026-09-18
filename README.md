PRECO_INGRESSO = 30.00
PRECO_PIPOCA = 20.00
PRECO_REFRIGERANTE = 10.00

print("COMPRA ONLINE DE CINEMA ")
qtd_ingressos = int(input("Quantidade de ingressos: "))
qtd_pipocas = int(input("Quantidade de pipocas: "))
qtd_refrigerantes = int(input("Quantidade de refrigerantes: "))
subtotal_ingressos = qtd_ingressos * PRECO_INGRESSO
subtotal_pipocas = qtd_pipocas * PRECO_PIPOCA
subtotal_refrigerantes = qtd_refrigerantes * PRECO_REFRIGERANTE
total_preliminar = (
subtotal_ingressos +
subtotal_pipocas +
subtotal_refrigerantes
)
taxa_conveniencia = total_preliminar * 0.05
total_final = total_preliminar + taxa_conveniencia
pessoas = int(input("Dividir entre quantas pessoas? "))
valor_por_pessoa = total_final / pessoas
print("\n" + "" * 45)
print(" RECIBO DO CINEMA")
print("" * 45)
print(f"Ingressos ({qtd_ingressos:2d} x R$ {PRECO_INGRESSO:6.2f}) = R$ {subtotal_ingressos:7.2f}")
print(f"Pipocas ({qtd_pipocas:2d} x R$ {PRECO_PIPOCA:6.2f}) = R$ {subtotal_pipocas:7.2f}")
print(f"Refrigerantes ({qtd_refrigerantes:2d} x R$ {PRECO_REFRIGERANTE:6.2f}) = R$ {subtotal_refrigerantes:7.2f}")
print(""* 45)
print(f"Total preliminar: R$ {total_preliminar:.2f}")
print(f"Taxa de conveniência 5%: R$ {taxa_conveniencia:.2f}")
print(f"Total final: R$ {total_final:.2f}")
print(f"Quantidade de pessoas..: {pessoas}")
print(f"Valor por pessoa: R$ {valor_por_pessoa:.2f}")
print(""* 45)
print("Obrigada pela compra!")

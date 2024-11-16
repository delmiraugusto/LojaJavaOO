
# Loja Java OO

Um projeto de console em Java que simula o processo de registro de pedidos em uma loja, aplicando conceitos de Orientação a Objetos (OO), como **associações**, **enumerações** e **trabalhos com datas**.

## **Descrição do Projeto**

O sistema permite:
1. Registrar informações de um cliente.
2. Criar pedidos com múltiplos itens.
3. Resumir o pedido com detalhes de cada produto, subtotal e preço total.

Além disso, utiliza o instante atual do sistema como momento do pedido e organiza o fluxo de informações através de classes bem definidas.

---

## **Exemplo de Funcionamento**

### Entrada de dados:

```text
Enter client data:
Name: Delmir Augusto
Email: delmir@gmail.com
Birth date (DD/MM/YYYY): 19/02/2004

Enter order data:
Status: PROCESSING
How many items to this order? 2

Enter #1 item data:
Product name: Computer
Product price: 4000.00
Quantity: 1

Enter #2 item data:
Product name: Monitor
Product price: 1400.00
Quantity: 2
```

### Saída gerada pelo sistema:

```text
ORDER SUMMARY:
Order moment: 16/11/2024 15:25:09
Order status: PROCESSING
Client: Delmir Augusto (19/02/2004) - delmir@gmail.com
Order items:
Computer, $4000.00, Quantity: 1, Subtotal: $4000.00
Monitor, $1400.00, Quantity: 2, Subtotal: $2800.00
Total price: $6800.00
```

---

### **Classes principais:**
- **Order:** Representa o pedido. Contém a lista de itens, momento do pedido, status e cliente.
- **OrderItem:** Representa os itens do pedido, vinculados a um produto específico.
- **Product:** Contém os dados básicos de um produto, como nome e preço.
- **Client:** Representa o cliente, armazenando nome, e-mail e data de nascimento.
- **OrderStatus:** Enumeração para definir o estado do pedido (PENDING_PAYMENT, PROCESSING, SHIPPED, DELIVERED).

---

## **Tecnologias Utilizadas**

- **Java 17**
- Orientação a Objetos
- Enumerações
- Manipulação de Datas e Horários

---

## **Como Executar**

1. Clone o repositório:
   ```bash
   git clone https://github.com/delmiraugusto/LojaJavaOO.git
   ```
2. Compile os arquivos:
   ```bash
   javac *.java
   ```
3. Execute o programa:
   ```bash
   java Main
   ```


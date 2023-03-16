prices = []
while True:
  product_name = input('enter product name: ')
  if product_name == 'done' or product_name == '':
    break
  price = float(input('enter the price: '))
  quantity = int(input('enter the quantity: '))
  total = quantity * price
  prices.append(total)
  print(f'Product: {product_name}')
  print(f'Quantity: {quantity}')
  print(f'Price: {price}')
  print('-' * 10)
  print(f'The total item cost: {total:.2f}')
  print('-' * 10)
print('Thank you for shopping for codeziilla. Have a great day!\nprices in descinding order:')  
prices.sort(reverse = True)
i = 0
while i < len(prices):
  print(f'price {i+1}: {prices[i]}')
  i+=1
print(f'The total cost is: {sum(prices)}')  

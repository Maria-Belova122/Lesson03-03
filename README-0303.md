# Задание по теме "Распаковка позиционных параметров"

def print_params(a=1, b='строка', c=True):
    print(a, b, c)


print_params()
print_params(a='Alex')
print_params(b=25)
print_params('Alex')
print_params('Alex', 25)
print_params(c=[1, 2, 3])
print_params(a='Я здесь', c=5)
print_params(5, 13, c='Я здесь')
print_params(c='Hello', b=False, a=[11, 12])
print_params('Hello', False, [11, 12])
print()

values_list = ['Max', [1, 2, 3], 12.7]
values_dict = {'a': 'Maria', 'b': 56, 'c': [7, 9]}
print_params(*values_list)
print_params(**values_dict)
print()

values_list_2 = ['Hello, my friend', (1, 2)]
print_params(*values_list_2, 42)

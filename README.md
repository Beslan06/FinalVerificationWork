# FinalVerificationWork      

# Задача      

Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.
   
# Примеры     

[“Hello”, “2”, “world”, “:-)”] → [“2”, “:-)”]  
[“1234”, “1567”, “-2”, “computer science”] → [“-2”]   
[“Russia”, “Denmark”, “Kazan”] → []    
    
# Решение    

## Здесь подробно будет описан только метод основной содержательной части, как и в алгоритме блок-схемы. Вся остальная программа будет описана в контексте задачи.   
   
* Алгоритм: 
           
* Создаем метод возвращающий новый массив из строк. Метод принимает в качестве аргумента исходный массив (array) из строк и целочисленное значение (length), которое определит ограничение по длине строки для элементов в новом массиве.        
* Чтобы создать новый массив необходимо знать его размер (size). Для этого с помощью цикла перебирается исходный массив (array), и в случае если длина элемента (строки) исходного массива меньше либо равна ограничению (length), то переменная размера нового массива (size) увеличивается на 1. После завершения цикла будет известно количество всех соответствующих значений, а значит и размер нового массива.       
* Создаем новый массив (result) и обозначаем его размер (size).           
* Для записи элементов в новый массив (result) перебирается исходный массив (array), и в случае если длина элемента (строки) исходного массива меньше либо равна ограничению (length), то этот элемент копируется в новый массив (result). После завершения цикла новый массив (result) полностью заполнится необходимыми значениями.     * Метод возвращает новый массив (result).   
   
Для проверки работоспособности алгоритма создаются и выводятся в терминал массивы из примеров. На их основе с помощью метода, которому передали поочередно каждый из массивов и ограничение в 3 символа на длину каждого элемента, создаются новые массивы и также выводятся под каждым исходным массивом в терминал.   
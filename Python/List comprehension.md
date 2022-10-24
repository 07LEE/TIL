# List Comprehension

리스트 안에 for 반복문, if 조건문 등을 사용하여 리스트를 만들 수 있다.

## 표현식 + for 반복문

```python
result = [표현식 for 변수 in 리스트]
```

```python
result = [i for i in range(10)]
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

## 표현식 + for 반복문 + 조건문

```python
result = [표현식 for 변수 in 리스트 조건문]
```

```python
result = [n for n in range(10) if n%2 == 0]
# [0, 2, 4, 6, 8]
```

## 표현식 + 조건문 + for 반복문

```python
result = [참 if 조건문 else 거짓 for 변수 in 리스트]
```

```python
array = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
result = ['even' if n%2== 0 else 'odd' for n in array] 
# ['even', 'odd', 'even', 'odd', 'even', 'odd', 'even', 'odd', 'even', 'odd']
```

## 중첩 for 반복문

```python
result = [표현식 for 변수 in 리스트 for 변수 in 리스트]
```

```python
num = [1, 2, 3]
word = [A, B, C]
result = [i+j for i in num for j in word]
#['1A', '1B', '1C', '2A', '2B', '2C', '3A', '3B', '3C']
```

## 중첩 List Comprehension

```python
result = [[표현식 for 변수 in 리스트] for 변수 in 리스트]
```

```python
result = [[i for i in range(2)] for j in range(3)]
# [[0, 1], [0, 1], [0, 1]]
```
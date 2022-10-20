# LEGB Rule

파이썬에서 변수에 값을 바인딩하거나 변수의 값을 참조하는 경우 LEGB 규칙을 따른다.

## LEGB 규칙

| 약어                           |의미|
|:-----------------------------|:---|
| L : Local                    | 함수 안 |
| E : Enclosed function locals | 내부함수에서 자신의 외부 함수의 범위|
| G : Global                   | 함수 바깥 즉, 모듈 범위 |
| B : Built-in                 | open, range와 같은 파이썬 내장 함수들 |

## 예시

### Local

```python 
a = 10 

def child_func():
    a = 20
    return a
    
print(child_func())
# 20
```

- child_func() 함수 내부 Local 영역 a의 값 20

### Enclosed function locals

```python 
a = 10 

def parent_func():
    a = 20
    def child_func():
        return a
    return child_func()

print(parent_func())
# 20
```

- Local 영역에 a의 값이 존재 하지 않음.
- parent_func() 함수 내부 Enclosed function locals 영역의 a 값 20
 
### Global

```python 
a = 10
def parent_func():
    def child_func():
        return a
    return child_func()

print(parent_func())
# 10
```

- Local 영역과 Enclosed function locals 의 a 값이 존재 하지 않음.
- parent_func()의 외부 Global 영역의 a 값 10
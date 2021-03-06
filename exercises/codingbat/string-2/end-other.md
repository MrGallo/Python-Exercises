# end_other



**Requirements:**
```eval_rst
- :ref:`fundamentals:substrings and slicing`
- :ref:`fundamentals:if, elif, else`
- :ref:`fundamentals:returning a value`

```


Given two strings, return true if either of the strings appears at the very end of the other string, ignoring upper/lower case differences (in other words, the computation should not be "case sensitive"). Note:  str.toLowerCase() returns the lowercase version of a string.

```
end_other("Hiabc", "abc") -> true
end_other("AbC", "HiaBc") -> true
end_other("abc", "abXabc") -> true
```

This exercise was taken from [codingbat.com](https://codingbat.com/prob/p126880) and has been adapted for the Python language. There are many great programming exercises there, but the majority are created for Java.

## Starter Code
```python
def end_other(a: str, b: str) -> bool:
    pass


result = end_other('Hiabc', 'abc')
print(result)
```

## Tests
```python
from main import end_other


def test_end_other_1():
    assert end_other('Hiabc', 'abc') == True


def test_end_other_2():
    assert end_other('AbC', 'HiaBc') == True


def test_end_other_3():
    assert end_other('abc', 'abXabc') == True


def test_end_other_4():
    assert end_other('Hiabc', 'abcd') == False


def test_end_other_5():
    assert end_other('Hiabc', 'bc') == True


def test_end_other_6():
    assert end_other('Hiabcx', 'bc') == False


def test_end_other_7():
    assert end_other('abc', 'abc') == True


def test_end_other_8():
    assert end_other('xyz', '12xyz') == True


def test_end_other_9():
    assert end_other('yz', '12xz') == False


def test_end_other_10():
    assert end_other('Z', '12xz') == True


def test_end_other_11():
    assert end_other('12', '12') == True


def test_end_other_12():
    assert end_other('abcXYZ', 'abcDEF') == False


def test_end_other_13():
    assert end_other('ab', 'ab12') == False


def test_end_other_14():
    assert end_other('ab', '12ab') == True
```

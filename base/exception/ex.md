def test():
    try:
        a = 1 / 0
    except ZeroDivisionError:
        return 0
    return a


print(test())

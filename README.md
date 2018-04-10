# 18410
回数
回数是指从左向右读和从右向左读都是一样的数，例如 12321 ， 909 。请利用 filter() 滤掉非回数:



方案一:
def is_palindrome(n):
    nn = str(n) #转成字符串
    return nn == nn[::-1] #反转字符串并对比原字符串返回true/false
print list(filter(is_palindrome,range(1,1000)))

方案二:
print list(filter(lambda n : str(n)==str(n)[::-1],range(1,1000))) 

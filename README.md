
length = int(input('Enter the desired length\n'))


def pas():
    import string
    import random
    alpha = string.ascii_lowercase
    Alpha = string.ascii_uppercase
    num = string.digits
    punct = string.punctuation
    password = ''
    while len(password)< length:
        
        password += random.choice(Alpha)
        password += random.choice(alpha)
        password += random.choice(punct)
        password += random.choice(num)
    if len(password)> length:
        
        random.shuffle(password)
        return password[0:(length)]   
pas()

    

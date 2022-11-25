import itertools

lock_passcode = 2583
digits = list(range(0, 10))

for permutation in itertools.product(digits, repeat=4):
    permutation_list = [str(digit) for digit in permutation]
    permutation = "".join(permutation_list)
    permutation = int(permutation)
    if permutation == code:
        print(f"Code unlocked: {permutation}")

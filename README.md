def sort_numbers(numbers, order='ascending'):
    if order == 'ascending':
        return sorted(numbers)
    elif order == 'descending':
        return sorted(numbers, reverse=True)
    else:
        return "Invalid order specified. Choose 'ascending' or 'descending'."


numbers = [int(x) for x in input("Enter numbers separated by space: ").split()]
order = input("Enter sorting order ('ascending' or 'descending'): ").lower()

sorted_numbers = sort_numbers(numbers, order)
print(f"Sorted numbers: {sorted_numbers}")

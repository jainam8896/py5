n=int(input("How many Number You Want to Enter"))

my_list = []

for i in range(n):

    no = int(input("Enter a number: "))

    my_list.append(no)

while True:

    print("1. Count total numbers in the list")

    print("2. Sum and average of all the numbers in the list")

    print("3. Count and sum of all the odd numbers in the list")

    print("4. Count and sum of all the even numbers in the list")

    print("5. Find largest number")

    print("6. Find smallest number")

    print("7. Print List")

    print("8. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:

        total_numbers = len(my_list)

        print("Total numbers in the list:", total_numbers)

    elif choice == 2:

        total_sum = sum(my_list)

        average = total_sum / len(my_list)

        print("Sum of all numbers:", total_sum)

        print("Average of all numbers:", average)

    elif choice == 3:

        odd_count = 0

        odd_sum = 0

        for number in my_list:

            if number % 2 != 0:

                odd_count += 1

                odd_sum += number

        print("Count of odd numbers:", odd_count)

        print("Sum of odd numbers:", odd_sum)

    elif choice == 4:

        even_count = 0

        even_sum = 0

        for number in my_list:

            if number % 2 == 0:

                even_count += 1

                even_sum += number

        print("Count of even numbers:", even_count)

        print("Sum of even numbers:", even_sum)

    elif choice == 5:

        largest_number = max(my_list)

        print("Largest number in the list:", largest_number)

    elif choice == 6:

        smallest_number = min(my_list)

        print("Smallest number in the list:", smallest_number)

    elif choice == 7:

        for j in my_list:

            print(j)

    elif choice == 8:

        print("Exiting the program.")

        break

    else:

        print("Invalid choice. Please enter a valid choice.")



vienkarš kalkulators 


def add(a, b):
    """
    Saskaitīšanas funkcija.
    """
    return a + b


def subtract(a, b):
    """
    Atņemšanas funkcija.
    """
    return a - b


def multiply(a, b):
    """
    Reizināšanas funkcija.
    """
    return a * b


def divide(a, b):
    """
       Dalīšanas funkcija.
    """
    if b == 0:
        return "Kļūda: Dalīšana ar nulli nav atļauta."
    return a / b


def display_menu():
    """
    Attēlo kalkulatora izvēlni.
    """
    print("\nVienkāršais kalkulators")
    print("=======================")
    print("1. Saskaitīšana")
    print("2. Atņemšana")
    print("3. Reizināšana")
    print("4. Dalīšana")
    print("5. Iziet")
    print("=======================")


def get_user_input():
    """
    Atgriež:
    Tuple ar diviem skaitļiem.
    """
    try:
        a = float(input("Ievadiet pirmo skaitli: "))
        b = float(input("Ievadiet otro skaitli: "))
        return a, b
    except ValueError:
        print("Kļūda: Lūdzu ievadiet derīgus skaitļus.")
        return get_user_input()


def perform_calculation(choice, a, b):
    """
    Veic matemātisko aprēķinu, balstoties uz izvēli.
    Atgriež:
    Aprēķinu rezultātu.
    """
    if choice == 1:
        return add(a, b)
    elif choice == 2:
        return subtract(a, b)
    elif choice == 3:
        return multiply(a, b)
    elif choice == 4:
        return divide(a, b)


def main():
    """
    Galvenā funkcija, kas izpilda kalkulatora darbību.
    """
    while True:
        display_menu()
        try:
            choice = int(input("Izvēlieties darbību (1-5): "))
            if choice == 5:
                print("Programma tiek izbeigta. Uzredzēšanos!")
                break
            elif choice in [1, 2, 3, 4]:
                a, b = get_user_input()
                result = perform_calculation(choice, a, b)
                print(f"Rezultāts: {result}")
            else:
                print("Nepareiza izvēle! Lūdzu, mēģiniet vēlreiz.")
        except ValueError:
            print("Kļūda: Lūdzu ievadiet derīgu izvēles numuru.")

if __name__ == "__main__":

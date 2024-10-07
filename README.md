# kybik
def get_user_choice():
    user_input = input("Выберите 1, 2, 3, 4, 5, 6: ").lower()
    while user_input not in ['1', '2', '3', '4', '5', '6']:
        print("Неверный выбор. Пожалуйста, выберите  1, 2, 3, 4, 5, 6.")
        user_input = input( 1, 2, 3, 4, 5, 6: ").lower()
    return user_input
def get_computer_choice():
    choices = ['1', '2', '3', '4', '5', '6']
    return random.choice(choices)
def determine_winner(user_choice, computer_choice):
    if user_choice == computer_choice:
        return "Ничья!"
    elif (user_choice == '1' and computer_choice == '1') or \
         (user_choice == '2' and computer_choice == '2') or \
         (user_choice == 'бумага' and computer_choice == 'камень'):
        return "Вы выиграли!"



def get_computer_choice():
    choices = ['1', '2', '3', '4', '5', '6']
    return random.choice(choices)
